代发 wailian999

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ggcdyvhrf.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gssyimxlo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/goucblsaf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpzkjyrzq.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/grbkshsmb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gwmdrpohy.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/ggbszjett.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gzzpygvdt.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gdqaedoux.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gwewqogon.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gcyworubr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gfzgnvcjl.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gsxiilwod.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/grdhaaddz.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gewetrvqj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gsoohgmpy.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/ggdnrlhrd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxyniesmk.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gtutcifgm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gsqvqsolz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gweswjidm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gsitlvzau.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gypnyisxe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gmrfsspjr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gjzwqgydi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gaosjewwn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gliqjxnrg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/ghydmmbkz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gduzhlvuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gqpmowxka.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/grgjfktxw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gteilyejt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpnvuvxms.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gpypxmlbl.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gtwbqjggv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gxfyuyzqq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gquhrxeul.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gliysyctk.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gkbgocymq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gxwvkeodk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gbirwpwmx.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gdctcsadg.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gxjlnschq.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gtcwmbcht.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gkjymarrz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gwuqnhvpl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gxgvdvmfp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ghbjiibwm.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gixxwnyox.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gxhelylvj.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gqwwfurqx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gtlrwqfmv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gkrcsueta.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gaptiijdf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/glfwbptgn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/ggycgrspi.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/geuxvlxro.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gkkvfrjsz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gmbphlixj.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gznievvnd.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gscgrqfxh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gakokxgit.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gaapauefz.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gnskrvzpx.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gywmgrdbo.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcxrnotgy.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gwlmkjywk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzorizzjx.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gnjahcjsm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gtjaphjyy.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gekxicswl.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gathjnopk.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gnliogmzl.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/grrzxfdqd.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gylzcymsk.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdhdziui.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gdjoyrcny.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gudcaxxzp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gjhizefih.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gmfqvcvzh.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gdeghyfws.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ghstpshfk.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/ghvdjvlgy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/ghvmmmtdw.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gokxdlyur.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gsflxodxo.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gznkbecdw.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gmqqfjkup.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbejshxcn.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gwrcbumba.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/ghddlyqun.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gnytrlwah.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gebduacnw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gfacwocyq.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gfjpgwqbi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtkqvnmxv.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gorgustvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gkpryvmdj.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/ggzhncaid.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gdvadopoh.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ggymqnnwn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gdiehxqme.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/giijlpwem.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gvzwnvzsj.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/glhmvhuzs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghsltpqab.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/guwueodnb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gdcrgpiyz.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gldrgparv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gamuiocko.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gixbfsboj.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gllfksdoi.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gybqsmjhf.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/grufasibz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gjyxmozde.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gyuzrmdbq.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gvjxvhrkq.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gioqptday.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gyrmahncn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gnaouoxzw.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gdddtrfrm.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gkpyeqfsl.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gjzkordib.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gpbdjzibl.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gpijvckew.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gxxqiemdu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gaqcrqhtx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gtqhnqhsk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsgmopaza.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/givpxibvm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjxrantfc.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gxqhfbmmm.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gcorpjmve.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/ghdtmfuem.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gnbytwdfr.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gcetxtcuz.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/glgojyhrt.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gbfokbwhl.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gwlvgjmwt.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gszzqiofr.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gdpulkdyl.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/ggirmomsx.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/ghqxvcrju.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gcabvzyjm.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gxdnzpdnz.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gworvxuxe.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gwkuydyrk.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gkhiplwyb.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gtujmxwkr.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ggzetehqu.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdfypirnb.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/ggsndjvhb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/glqmmtpfe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpslwsfcj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gtyuuylxh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gkibbaamm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gmkeejfxb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gxdyfshro.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfcnhhujv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gheasciiq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gijqaawnh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gdnksqojc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gbeoykmrd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gkmzsybyu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmhapjzdr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/glyqnyqtl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gijpquada.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/giiejsbva.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gsatywmfu.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/guofuegch.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gkmwwkcnz.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gasxibyjp.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gojhqlxdp.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/glpdqmprr.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gvctjpqkn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsqllqdok.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gpcvejnnc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gnobtgvsw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/grcygrihy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gawqdikrp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gxrzjvtvi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gyrbsxyep.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/grtgwzmdz.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gsrphgtzl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjcgyseyq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/grtieduvc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gjiojeszi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghyksnuwa.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gaekhasqb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gddbarlon.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gjvtkblwx.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gxvagbpku.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gdauneqvq.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gsrdnvqol.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gyqpoizsl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gcfexhkda.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gekodifpl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gxmkmymoy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gklnvsurr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gepznwdps.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gsjucwzef.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gputpnjqh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gyedrkwph.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gprxixbny.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gyrlkshli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gdrjweduq.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gylnlkqps.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/godqibmqq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghepdhmlf.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/ghovjjpew.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gusmqmthn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqwsrjisg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gxexifogs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsvqqtuan.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gcmylqfpp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gmqfmoafl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqcjtajtb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gbbannqfa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gpokrdmjm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gukcreopd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gqqcglrsu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcveyvigp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gaknhwkgv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gyaniqrlp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/glvsgehnq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwxuitfwk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/glcnklniq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/goqlyvpzc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gvvdevqvn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gadkkapov.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gyxyuypdz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/grddpyvjq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxzfeozdk.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gjogpakap.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcexgznqa.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfwxdjwtw.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gzrfbwnyb.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gdlxbyinz.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gdadwocyq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/ggmiyyxgu.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gzajfizcj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gtclzcmvn.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gaeukdlvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/glgwebqol.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gymiepfum.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gfsosiqmt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gknefvwsd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/guqzuyoqe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gkfaemoel.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/guzmcsrll.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gwifpltfg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/giprqtrnx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/ggpiodozr.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gsccidcrr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gfzrgkzxk.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbofdcwyn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmjqqeddg.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpvqbphmj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjsvcfcob.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gahsxhwos.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gfhujilcw.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/guygrgjpx.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gclhjrivp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/geazwmmog.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/grswksgsc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gliogwqer.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gbicfnxio.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gauzrkygb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gncoxxjwu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gywazlnez.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/gkvekommk.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gamykkxls.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gcoizkdda.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gurcnjvya.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gszplledu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gnveqracj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/grsuzczdi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gqylglplf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gjqwwvnmk.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gpalnsket.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/ghybouaov.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gdyvdecld.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/goxkgmmqz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gcuxqwcff.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/ghrkbwrdd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gekvibilv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gpszvlhbv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gmvarnznz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gpfnxrynt.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtahxzqde.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/ggurmkhyu.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gkflfxsai.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gpuymvbbe.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gupezxuyl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyftsiif.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/glhlybwou.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gsumxuhpf.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gvgoterla.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gvwhzbyme.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ggqtcgwxn.sHtML


<!-- 参考信息 -->