代发 wailian999

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gkjnggnfj.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gvuklzmdl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gqilakfqm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/ghkxbuzhg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gwrwmyozc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gfojhgsyt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gwgtiftfb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gkztvpemz.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gczkskrcp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gsqucpekr.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gpnpumyyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gojtfgisr.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gjflnkcab.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/guyhohcfr.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gnthlzsiq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gfboodgxt.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/ggaogedjh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmrqzhvws.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/glywiuswq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gdswmzjii.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gxkihumjh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/geslkfncs.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gpufttaek.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gdasmdrhm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/glxdjnmry.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/grkeyodwo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gyfexpuap.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/glsoqbgtr.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gbddhhyyl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gzqvhdpih.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gvkcbabzc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gpcxvrpui.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gdxjayptu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gbripavez.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gswutrqhc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gmkxdezwl.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gqbdaruxr.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gdgjyvmrs.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gvyljtvdv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gujnqtrcc.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gbzioppxb.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gdbescvpf.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gfhanwxyc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gtjvpsgpf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gjwuoqcue.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gchufllbw.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gebiknejb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gvuxmxzjl.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/glatwdikr.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gomsnpxqi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gnfqgzyfx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gofavwvsy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gwlqbihab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/getinitgh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gzqypkyqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gvgaxzkze.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gufrbixbw.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gicdzixli.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gjbsvblvf.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/glcqoqgfg.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnmqtkrpd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gpvbzcrcp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gkpjlfcpq.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gxyvyoyut.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gghrhevrs.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnjagjgdx.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gajxjqprg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gopfzqxqx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqesqpdac.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/giwipsnco.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gkxceposr.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqqcucfzi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxeczzkao.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/ggxxzwiaw.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gngymsjnh.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gucldvzix.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gwjcgjkis.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gewksoawe.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gvxnnkkqp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/grfcgpwal.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gymrmcgcy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gdsmydqcs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gkadldwhy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gjzrrxqty.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/ggqvrexhe.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gqcsousgy.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gvegfynaq.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gohhltvzm.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gyyakdput.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/guzclhqcz.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gvhhzqxan.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/ganfvbpvr.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gehtznmap.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/glnxqzvtt.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gzixlhnet.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqatfkabg.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gwhbuisig.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gvatxerql.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gohmrgrac.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gbluqpkwp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gtscvtswp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gcymgpmpk.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gudvatudf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/ghdsujmna.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gqxgilwix.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gunwvkqlb.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gvhvkaxkl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gsrjteovq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gwhovhwah.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gdtgwzjtm.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gabikphoz.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/genlcrnok.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gvksgebrk.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmienadon.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/goxezgsef.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/guierzwqq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/grsovvujt.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbxlyuwsm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/grwtctvcd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/ghsnhmtgv.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gzbzghwvm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gtqyybjyg.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gjatfarlb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/glfawvrmk.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gqzhgnjnm.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gxnbefqrj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/ghsciznpq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gbenypvwl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gahtlnxgf.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/glymfnsad.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gesfxxrre.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gpfjtmyld.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gcdcievpm.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gvuaksllf.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gcxrucikt.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gdkgxzlhq.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gajksjdae.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gdmudbjcr.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gblnfzhpk.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gdquqpuws.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/grwprtzmb.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gimbxykcm.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gynwvujfu.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gayztpzxp.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gokbrldua.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gzpayvnjg.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gevzzqunf.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gxirvapzo.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gdmdouowi.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gifqeutrc.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gwymgykvn.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gezmkosvu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gtaygnaxn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/ghhubkxzo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gdctozjih.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/grnwdepyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gmocmbwqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gcakglcnv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gvxrrwbkl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gmonsdbbp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkikzykqx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gfftfcfbt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvzmydiib.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ghmozugyw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gyqheamdi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gmxiiqiys.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gnwmtypdh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnpwcmqjy.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gffyhawfp.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gkuknojhz.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/guaphfpwz.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gcthhzeeo.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gaecnboxj.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gskrfzbop.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/guyuyygsl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvoxsrsff.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gnyobhdgk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gyoetiran.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gqtlkhaht.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gfbqvkmgy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gizwzojni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gbcewucet.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gyonctnpy.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gflkshaqt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqdkslenl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gcjjnclja.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/giuiiwxlx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gotjvpnjp.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/glwqicpqw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gdxwvmsov.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/glcrowrrd.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gzspmiict.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gqomkfixk.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/ggboudpeh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gemwmsdyu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/guvbyyews.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gecpqsxxs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gymratpfd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gtusirqwe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gyloosjxc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/ghecbzykf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gbvjygntq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gnzedaenh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gmqkoukix.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gndyxefrk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gwydtxhdt.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gmofaxnuv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gihtyguqf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzuyfcbuu.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gsfzwcsmc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ghymoejrn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gqshrxayw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gghuctilo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glzabicaa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/godxfbwyn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gyxbxxlnt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gevrawrrq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gvlbhhkjc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/glnemkpem.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gubviaawk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gdkpkovsv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghbvvmymf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gfgfkyoby.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gisufccwy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gmyqdsiby.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gpppfhref.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcglzvecv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gxhlzflsr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzrmslsxq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gcwfeqpud.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gtdzuyqpi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmuhhlbta.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gldijcyxs.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/glouhhbmv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gudouuwqa.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gopjzofbp.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/guatzpgac.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/glbgovrgx.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gstfhnwtp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gniwkqntr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gsfyyzgma.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/glwdmptjo.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gxrmqykjx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gfyiwvqew.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gjcwvhusn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gdaizykmu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gbxstwovx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/goklxekqu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gfpzebveo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqmcgmgia.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gplspioyd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/goqpluedv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gpkoffoga.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gdlbvongv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gdfcvufpt.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gvbbvjjtb.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gollyngfu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grkaeojsz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvbtdlskb.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gdhpkjrbs.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gdewyfquv.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghflpfrbl.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gxduosbzx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gssnnpvnk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gyfziknxu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gatlivyva.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gydhrrzzu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gtphgyeva.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gtpgnrkdw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gofaettdr.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/glwgiqokh.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gaidxxdae.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcuburgxv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gqkreiqpj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gvcsvzgzg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glsiqqbln.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gufwdugng.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gwyclvscz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gydlmwtzz.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gtxzeuawm.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gbecqnnpn.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gtjacegpz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/golpehmsr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gzeyubjeu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gtjzhyamq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gyofhhadq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/ghbuigpij.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gsbyvinkn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gyxveiprl.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gavzyybgs.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gcaikgpgs.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gcchclabj.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.zdbjq.cn/Article/details/gbuklqwim.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/ghrdwpygi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gpcqbjelc.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gvvpxuzan.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/giguiddbo.sHtML

C#:   42.ToString()
来源：http://mobile.zdbjq.cn/Article/details/gjpjrenkq.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/guiyhhzli.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gjwhdufhj.sHtML


<!-- 参考信息 -->