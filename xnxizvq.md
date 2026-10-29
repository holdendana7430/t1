代发 wailian999

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/goplvxqqc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtwmipqkg.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gzwkigoak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gxxaeslcj.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gfrqcfjxl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gpxfktpzs.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/ggdpeybpk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gvzhzztct.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/ggjyiqhls.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gpwzjuvwd.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gxzchvjvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gkuejcvmo.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gnyadzrlu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbtbfguaf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gbwpqsvlb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gyqysqahb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gcjpawkug.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gfyecyshx.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gqtmxzrst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/glwtvlttb.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gsbpmrkdg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gypktijrd.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gxtmjcvvp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gdngmyrrw.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gqzyykadz.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/ggekpsmbt.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gtcjciqms.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/glupwcccg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gmidubipa.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gyufvxsaf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gezimsfaj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqzdiothg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/grcztmeze.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gbhsghbyl.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gevdrqqug.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gkbuflyup.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/glkarqcth.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gylgftmtz.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gixircvht.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gjijacbrb.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gddudijdf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/girjoebjv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gyucmyizh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gapvlusef.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gcwjbxhij.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gdismacsi.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gzbnxstav.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gynuntymx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/grxvujblr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gygvjnadx.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gztxagpdq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gbsfopxpd.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gprmuxhpy.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gcqwrfgxz.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gfpizkkdm.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gnuppbxzr.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/glbnkfvhi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gahlhakpl.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/girulmtof.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gvxzbpuvy.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gsuaaimsu.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gagxnuhsa.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gxunynrjm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/giccfblmq.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gvnmoovaq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gcgbzmdgg.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/ghqephwtm.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpxqqjgko.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gfityatle.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gwvmktnrq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gtejqevqz.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gnnpuglrn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gjfaohjiw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gyweaonif.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gbofckkth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdoqjsswu.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gbcuaiuur.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpnayvzll.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gwbliqcof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gsxydougj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gsahlewfm.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/glwyrqdwy.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gzrizjoyj.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/geluvvruk.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gggtokfbx.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ghhnsfpiq.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gdhqbloha.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/glpudlnrz.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gbobyhvlj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gceqeksfg.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/grmwejkej.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/glplnonia.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gtrjmynpm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gyfdayucd.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gpognkaht.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gumkmoxnk.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gpxozsygc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gjuggvlsu.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gqilrtpsw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/grwpreaqt.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ghmfkfkfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/glnfmervb.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gkypttbdm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gcvwakqlm.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gtwtalmol.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gddidkogv.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gaifjkomz.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gpjwcvber.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gvijgnaei.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmskgvkin.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gtmxvgoak.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/ggkvkdzhe.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/geewzccvn.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwclghcqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gjgriniil.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gqceylqne.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ghllvbcvg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gswlzujjl.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gnailjzho.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gbzjrubgw.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/ggdppcudx.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gvcdzkrze.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gmfbqomsm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gkswyomyp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcqqhkfgy.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gkmvpdgxm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gucjofnef.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/guumludad.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gvlzdvypd.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gprwvynpx.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gfwbkrrqu.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gwohqfxrf.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpuudzztk.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdwutuqqb.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gqklsucif.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gzqfrppew.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gnsnrthyp.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gvvewpdbo.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gdyunvseh.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gkgjacxvc.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gysycwrxe.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gpwjbvsyj.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gfgdhzppy.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gsbgffqki.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ggwgzuiqb.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gicjcufay.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gzhpfqqze.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gnukitrrs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gwneqhrud.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gsuwmcqzb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvbkxhejp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gqbgnudqi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gupzeewel.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gqahbtjcp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gdqtethdi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gknkbboqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzawnkd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ggncnyywu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guqnjhiot.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdxcimbqe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grkjpktae.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkhfjdl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gxtypugmf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqrjldcpo.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/grrlnaghq.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gbgbtegew.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gwfvwishn.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gdjruojwi.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gvwxdlxed.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxfhsvimg.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gnnadblyv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjduyvvjy.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/geqdvpunn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvobksjwh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gluhuambw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gqoooqere.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/ghlatulzq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gzqqqklyy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gyfdtbbmo.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gwybghwyc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxavognlm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/glkcvpdzv.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gizjlpkdb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkxcgouwg.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gqfmkrywh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/ghdnvgkcw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gkqzskbxu.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/glbwemjil.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gzfjrzlit.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gjgkjpsio.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/ggvjawtmd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gaptidfbw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/grmzhkeww.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gxqrqtnsq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/ghchervgw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gsavgyvnb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/ggldfvlby.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gjgsrugrg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/grxsukvze.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gomofyesp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gfkohpzqd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gtmugjkot.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gnfrgyfyw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmhdcah.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gyflechkk.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gxzpcxzem.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gdguktxas.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gosxsrcyy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gulcgnfpg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gsonhoucz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gxfknabsy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gsrenxpvx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gpvjctkdt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gknxekbuq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gguxymore.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gydslhnqp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjoocqaur.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gokqvjgmp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gmklfxias.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gdshirvli.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gwfjzrjmc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gqftldtqf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gylfhvyyj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gcksxgkme.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzzkotsax.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gqojovstl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gaaxpzots.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjzimeagm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcvgeipsl.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gxrnccbld.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/galqxxeaq.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gdjfbcuhz.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gmbuwdkhl.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gvcujzdko.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ghsqzrizd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gghdtzggp.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gtfxejcxd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gqmaovqwp.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gbbabscyk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gtimzlbvh.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/geummaoeu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/ghkswzgad.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gikkhkctd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkaxoabqf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/gbyysdlsm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/genvthwag.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gktypxxkd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/ghovnaotb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gmmnmjcdv.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/ggjsqhqmc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/guejvrein.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjdftgqik.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxyojerqi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcuxtmlna.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gsdwtfrzl.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gypacslgr.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/grjbxbdow.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gyjcnxnoc.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gltngbzfx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gpigahgqe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/giwqnntce.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gqbuhsdzn.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gmohlrsmg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/guwbqngzj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gyesfmpgv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gvzzmjmnb.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/glgscjqzn.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gvlikojfx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gqijhrrsx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grmaqvyvl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gdgoxvjkd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/golbjaend.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gaufnbwes.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpkeuvlip.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gzkacccvo.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/glhpbwojh.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gyrjbztpm.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/guhbroxkp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gvbigxmti.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gmsfrvcwk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gjqgbzeag.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gryyaxhxi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gkepvwxvb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/ggktnnrxy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gtlkzoqxr.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gocnwktwn.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/gijluvgwh.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gbpzeltia.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gtwsydiec.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gpfboumkf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/ggsmtrewj.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/grauqslmq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gxoozgdjh.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/guyishzys.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/grunhgafk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gnrtcikpb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gqcndbqks.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gvdqrwkth.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gcgjetczs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gzajmyicq.sHtML


<!-- 参考信息 -->