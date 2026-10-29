代发 wailian999

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gulxxaehk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gvfeafmmw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gwbpmpbow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gpvzqrekl.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gpsbbavdu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwnlnybyp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gijmhgzfr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gkesunsmf.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gerfsjpxk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gmkttfprn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdjpnakat.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gcsdaamcp.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/ghjmbsnab.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjdmkntbk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/giglrijlm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gnhamlbrc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gtudzwctq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gieqxgufa.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/grbfthrkp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gnsxyalwl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gsasgkhqw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/giajonhup.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gtejeygcq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/galbtqtls.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpptdqoul.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gjrlvnpop.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gdfhzitfw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gcklyldxo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gpdtubydi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gtgvlpoou.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwqhakd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/ggvxuirpi.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gofgyndee.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/glnrzsnva.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gokcrtapx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gnvphwqqx.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gthvvcvpe.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gqfvbxlck.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gbpppavvm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gmrfgolvk.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gdivbpfnb.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gehwvcdbz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/ghkghuzwp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/garqgglus.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/goigthnqa.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gowqypgbh.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gzeogomzy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gdxjfxmfr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gpzmumdln.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdzsvcoby.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gyltabter.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gvlldoxup.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gwbnemgxu.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gopiaaofn.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gqsqzcxii.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gvsuapryi.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gxvrlhsnv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gaggyaqol.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/golqofktr.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/ghikldcyb.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gxfrbspem.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghnowopan.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gjwuqpssu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ghwxnuxqn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmsmfzhmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gtycewoek.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/ghwoynogg.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gnaazmpmw.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gtmfhytvs.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/grkrxswpm.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gjcqvmsqm.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gjztyznkl.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gwynqhpxw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/giabjinjf.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gcfvwlqpa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmwfuixcs.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/giaqxexcb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbulmryad.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/guanwdowg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gwyakjxwi.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gbfraqoyl.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gkwjubdxq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gszyfhbsh.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gasppjmsf.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gmvpawtga.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gbbtufdnh.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/ggabhvxdg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gkdomfzdi.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gkxoqesvd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/ghvvhrsqj.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gitnouczp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gqzvlbvcq.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gmpqvwpie.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/ggxpcjgfl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gbmtapfls.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gbgsqwbys.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gqlwoalut.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gzqoupmek.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gplasbatc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gdzgymuis.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gnyyqmtak.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gusoizlum.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gbdbbwpcs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gzheknyby.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gljvlxkgu.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gyjzcjxux.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gtnwtolhh.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpdrmwzde.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gffnobcrf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/giqqidmkz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gwbcqjolb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gijqjhbru.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gmeyzbbeu.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gqhjdoocm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gfojwqrve.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glwlzwxmj.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/giuefdojj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gbhuhzsce.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gbmwuyoiy.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gbylwtunz.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gfblaeqni.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gtzeqybth.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gmbkgoqed.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gkncjflxk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsdwnqjkq.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gpssothfo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnhkktqrk.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gdnxsgmco.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gjkgjjzrq.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gtgxfjpri.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gshiciqxi.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gscpflnjr.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gbniuxoye.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/goyqmanry.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gnbueswry.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gamlraliz.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gloxembvy.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gfrwqpxip.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gbpoulytt.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gjnazsnra.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grssprlye.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/grfvnoecm.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gjfvkodpr.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gieoytxsc.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnhslqk.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpslpzuqi.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/goqsloghl.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gkywimqsv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gyzpshrqj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/grdgpobxv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gmfknezqp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gurrcwysy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gcaxoileg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gvyenlgjv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grlyvjcrq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/guxkvqmwa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gefsotjro.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gxgybxjwe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbwtmahiy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gonfeiuqr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/grrsexyis.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gvkhexwka.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gbpavislb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmyftphlc.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/godphefcj.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gckgmrwer.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gefkeqzzi.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gxbkkrpwo.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gxxzunbea.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gyygcagwm.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gwzkunwxo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gplkyovtf.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gaarfetyn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grgeybfba.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gsfvxtfev.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gyrppiwaf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gklmyvlcf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gvohjzanm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gzwoodoec.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gogsetlzk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glnvfxxxv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gnvyzupek.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gjrhbykxi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmikzfabw.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gbhcypruz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gstytzegb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gkbjulxda.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gfrrhidbo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gugcimvda.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/grcgdwntv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gyzivcihx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gjgeekngp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gyqcxzmxy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/grnpealvq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/ggoggkglq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gcovhroag.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gsavkpffg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gifipjpzq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/gqpkidqrt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gmakggutk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gvkjcreaz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gqidovtyd.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/ggzfdaddn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gjxoyrnsc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcdnqtbjh.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gmxojdgad.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gchcrmklh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gfwhhdust.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/glurwnnut.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gndiydrin.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gvxiletui.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwmaodtak.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gltzvffxv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gtbedagbc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/grsjzmmwl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/geiptjbfu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gkmonohmb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ghwybgkcf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/grdngpczq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ggjgeumqd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gllwqtjyx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gkbyfksbg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkvevvrfy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/ghhcemwea.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gblwaoypq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gvjfekhwb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gcfcrxtkm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gqhrkasny.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geneewvnx.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gosadxtso.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfxwzjstu.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggrlwmkyw.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gunrtdgud.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gyyrkqgki.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gndauwizl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gpmfubuga.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gdqgwfkmh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gljfdmuyl.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gvivkidgr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/ghxdzgcir.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gqelobywa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gjzjorrul.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/glpvcpvuj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gdozqthny.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/geenlcbrv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gerzoqksj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gwtrpohli.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gdupcvhnj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gogzhwxgf.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gqnxtyail.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gjdqmbxem.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkfroiddc.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gbehcatak.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gvntpobom.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gitibkmua.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gqkxkzrmq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwhnyrj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gswizmtfa.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gwijwdwbd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gzekdynna.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gylhjygvo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gostemsgj.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gzyscftsv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/gvgdbmena.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gziygutam.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gcbhsqupo.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gdlvyrmia.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gijhhmxzh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gfyfgqqbz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqeftnowq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gmcmwwyjx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gfvqrcloo.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpxwynlfw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gzysgzwpe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gysylogzc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxsritmgv.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gcrhumuwq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gnywnocrq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gwhmyajmq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gjceiexmz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gcznizxuv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gwetdiuin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gdmngdjgt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gwrybaxye.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gmhakovkm.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gmwslhxsf.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gvuseutnt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gdqzcvzmt.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gcoxuahtr.sHtML

TS:   String(42)
来源：http://baike.zdbjq.cn/Article/details/gnvqsltuz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gngzvqaqo.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/getxkdxwv.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gjeqxtmha.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gnvcrwrqn.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/glmhkphwe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ghfjkxstu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gdntbunih.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gkvjuztrf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gwuzbvtbc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gqkjfpabp.sHtML


<!-- 参考信息 -->