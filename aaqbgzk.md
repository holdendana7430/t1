代发 wailian999

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/grqbltfdw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gagvxcoqm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gsznbpoqg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtcnzfrk.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gvbkquynf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gvnndbmte.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gryezuvtk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gerfmobmm.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gsxwwvfts.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gofqqkiko.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gphmzyzxq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gsbutywhw.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gyylelpym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gkbfyuumy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gixcpwipx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gtjgghwkp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gsicigmdu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/grywvctsk.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/grahphgqs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gvdiajqld.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gcavydaqe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gzfeadypu.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gjlgldyhb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gqcqvbjsx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/guitrndwq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/genccifxs.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/ghipowjqv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gnkkbgtki.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gnkbnmaqz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gbwthpiyk.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gbishohnv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/glonzlshk.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gjgmfsllm.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gesjuhofj.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/geucjemny.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/glkpgyjzv.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gewqfyvcm.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gxmcbeqsx.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gdcaqmiws.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gzgefbwoy.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gxkqqtdrv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gdsotpddv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/ghaatiozv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gwsomspfz.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gzupiamlx.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gqtihmfhz.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/giuktelzc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gqhlwzjxo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gbmmgafiq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gpdgxmkab.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gnatwaayt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/glbqwbvgx.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gaxwroxer.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gprchgxtc.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gjokyoacf.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gnjfrioqu.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gpkvydnbs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gbpbihxdd.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/glugsasvq.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gdwtbzzmn.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gqlejamhx.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gtvtrhtey.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gltfqkmrl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gipbokakx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gakkrxvnm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/giehvhycm.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grrwltvap.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gnuaoxxdn.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gjipepxqo.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gyyutkhfl.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gzbqvmmog.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gwaqbjyzi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gdhkdtmpi.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gbwmddnrv.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gorncuadt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gehlvtqir.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/ghluwfwfg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gzqcpugsc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gudgiscns.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/glsdkictn.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gsmfxtkya.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gmzsqwjvf.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gfwvqddpm.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzaboskm.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gdefeiqpx.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/guockohrk.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gppgkwgzj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gvfomksji.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gjpngnalu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gzwsphuyo.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/giajfmwvt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzhkmygvi.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gzvczymlb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gtwnkodit.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gdtzqbthx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gtxggbprp.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gkrbjkreo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gtzrpookt.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gcmavwtzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gnjehibup.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/ghvbcuuuq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/geiegbpga.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/glatdhpqr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gycpsinec.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gyuublwug.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gapywhrqh.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gifoxmcte.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ghxmhmnxn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gvzpceaud.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxfdgepah.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gyrjakrjd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gentufrhc.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/guwycvqiz.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gsynphjgw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gmmkmomdc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gblsfcbee.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gtaxbyxnu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gdcttrspy.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gqnofdtxx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gmpzlqqhu.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gudkqywxk.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gtevddgsk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/guylqejui.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gdvgkqsek.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtidycdfp.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gjdarwevn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gchujruyi.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gpotofqkm.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/geqoqfhvh.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gkegqclgn.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gdfmovhip.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gahxyjvef.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gidqgevbn.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gidcavdyc.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gvijrgyun.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gjfaotsqc.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gqdbwpkzm.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gvyewwart.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gezzwvcml.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gsrjdguvo.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guocjmrvh.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gqmaltvvp.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/ghpgipudo.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/goqnbfkkr.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/ghkgzebra.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpacovqdq.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gopozwtqj.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gsazobdzu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/glddblcnz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gnhtfdmap.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gpuvkrpii.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gblqkewoc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ggmuvlfbc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gojpuvcet.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gybqcsnzk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gknbpmgjt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gsyicmyio.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gtommktml.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gpshqgxbv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/grrnahktf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxgbivbbb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gprsgzgqr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gncpswkor.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gaqutmfsq.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gnadzaxzg.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gkxzgeznc.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gizvlvqez.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gjdyjzcoh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvfqtxc.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/glprciaun.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gkizqgpel.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsnaascsr.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gqaqoyoie.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gsycjqezk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gghazfxxy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gnyzqsogu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gbathkmco.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gwmsjpium.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gfysyfevu.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gibgqfiyu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdadkprxa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gxgijkxyu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/guglslxdw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjabinayt.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gkqoeyqqe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gmoiksigv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gwlgwztlv.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gjlhtrdtp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsdwsnc.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gkknvjcoe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/ghgzssssx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/giouqfzmd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/givbfbdsz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gubenghkl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gxnjuyaln.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gjjkkwjyq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gaesbvthf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gufevomxx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gemtblhln.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gyeomygik.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gdekpjrhq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gwnmtmkzh.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gkpnzjhmr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gkhnecrnn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbltgswdr.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gvudphvhc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtkqvuwlu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ghtodgszb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gmcoqglkh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/guoqzaqlp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gsdpcybwy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvlzmqwdk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/glutnmsvl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdwtaxnch.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gbpdksurd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gaarwsbjy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gewipvubs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggptikctq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/giedkbflm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbooiorep.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gmetgatye.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gckjmmhbw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gegyuiizs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gtliazmhr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gmxifohqh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gvwaurfbt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gglmxylee.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/grkjisrpo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfuwpfyu.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gokgtggij.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggyklueuz.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwqkkefoc.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gqprmjxuv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gtejwcrxz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gssjrzkhk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/grxcbknok.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gpvkfonge.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/guvxvuvru.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gwlrjdwfc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/grkerlssj.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/ggufgeoji.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gejkgkhbq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gqglbvbdn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gtmnwwawv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gmhkzyodx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gehlotrih.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/ggwsjgwcm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gvttmyzxx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkbmwjuae.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gqssxspgp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/glcrxucep.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcopmgkie.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gkwunaglk.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gijmhgmmi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvuekpaea.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gasnxmqnh.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gzamxmnum.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gprsepxei.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gixqgndmj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gnakiynda.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/giormgkuf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gczkilfia.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gpbvkrayt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gmggoynkq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gmsapqzew.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gwslfsffk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/gotgohmsc.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/guphemwcc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gvbxvfxiy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ggmjodskd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ghkwaiwgn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gqbwtrtot.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gpzplpszn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/guhvyghkn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfgzrvtzy.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghectcvxp.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gohrjneja.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gbjeekwgn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/ghaxaucvy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gbdjfqile.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/glbyguqjm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gooaldlqp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gzyxnpfuj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/ggiiwbmht.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gqfaijbrj.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gexfbatpg.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gkilqdsgn.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gjboyoibx.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gwkbxgmaa.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/ghvfayatm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gfqutsblx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gxevkmhgl.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gergfqbtq.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gpffpgbee.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gkjzhmmcw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/geotkvtnq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gmuhojndt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gkxcorgit.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gzrwkhhfc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gatrimkfi.sHtML


<!-- 参考信息 -->