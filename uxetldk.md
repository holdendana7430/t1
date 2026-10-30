代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gzqohpfwv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gthbmrwcg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gfyxxdumv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gxqfebwam.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gcljjydjj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gtjultdzg.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gemaodbja.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/ghgmftfnr.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/ghzhfdjkc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/ghrvdoyrx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gsdornwgf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gbpgfqtbm.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gktnhupro.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gaaouqrtq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gffartgvq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gglnzlaya.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gscvntmlg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gxkdxwote.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gujpwbgar.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/grdxamkcy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gmevvpxmu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gqkaveqbl.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gsawnzoxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gmqnafmsj.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gsqfdrjqw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gdkkfqvjg.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/goayyziba.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gowfjhilh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gztpmimdm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gsdazwupu.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gqzhezcqc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gceketgiw.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gtucmgpxg.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gppumedak.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/ggjxkuymh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gtilypgbd.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gtotkqwpb.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gmjjkwlvx.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gfizjtvbe.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gshpbnacw.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gmzqkpepj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/ghctmqemw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/grrhdyfne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gekqwdrdh.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/ghevfmxry.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gnvugmpce.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gdhxwzmzi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfowymen.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/guzlxefek.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gixkgftvc.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/ggosgzzzi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gfjpwasxh.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gxlaxvhvw.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gunubbtjs.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gxbgjodou.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gptmiwwrh.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/ggcmnfivy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/glvoggvkz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/glfbpcyrc.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gypgnrapf.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/grmjxmzdq.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/glcprlkpv.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/girjtklio.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gtpscucyg.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmwvonc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gekdilbez.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/grsllmspn.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gkunuufen.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gabzwgsiv.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gqyfjfzhn.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gyiadvbgp.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gshaapuib.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/grfoqhxwy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gmvznmbdh.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gxvnfyayh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gkbjzsoqq.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gikxelzfy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gxixjbirw.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsfruauhq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gpeytyflz.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gmmfiwnoe.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/guskghhto.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gtoomwttr.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gcnynnokx.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gdigxdaqv.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gyqmdqhgl.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gphnorsxb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gxlbvddte.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gsqvcnbav.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gnceoqhbn.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gtlbdmokj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ggadaetcy.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gvptptzos.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gagzojtpf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbshnztag.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gemehcsfk.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gypsshxsu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gmeefseet.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gdhrlmdci.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gvbtqzhyh.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gkpepdhjb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbmrlfwdo.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/glmpzyhjf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gkgykyayl.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gbqazzerm.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/goigwegob.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gfxejwbjr.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdbueeoum.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gqknxcueq.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grdygkruv.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gotksbdjh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gepsfvzjw.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gowlyroad.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gdgqscwny.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gvqnczquo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gaiqzldhr.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gcepjhzna.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/grujerxbp.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gnmubaidn.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gwhbdwrnq.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gqszoucaw.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gxewzszdd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gvwqrewiz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gjxfpnqjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjwbuazid.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gownmuvbo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpkaixbkh.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gnzwwborj.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gzjdsckic.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gcakqyceu.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gtykzzofb.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gbrvgtjxf.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gzdzijcou.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gjvwmtntb.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gmoojedjh.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gbilninpi.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/guztcqxqw.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gywbjznwt.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/glqzcvcmx.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gwijwwxwn.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxwerowko.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/glcjeeeni.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gebpoldpd.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gdkkydoeq.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gctyzdfcv.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbrgayoge.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gltvnreae.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/guibshqkz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/glmqxesjg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gmtmtvbit.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gusjlqlre.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/glqkrgboq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/ggtlgmvyq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gzruvdluj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gnggpwizx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gcyfnhmtd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gegrbwutw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gtpnbfyvt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gwahnldgq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gimogarse.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gvxhordnn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gvkaurhvc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gmrhnvkgv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gsovspxva.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gkxdnssnr.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gcifokzvi.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gdwymixbx.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gyegpebuh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gaioalzsg.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gdozbrwns.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/grposdkic.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gawqqozlf.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gxtbbekvz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gddnebzrv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/glewbyqhs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gfljgdhfc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/garsbkwry.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/ggnmlkoze.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gqlxljblu.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/grxiibfwv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwtgkkati.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gxsszhsry.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gkunfieea.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqvnzyhzz.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gtvtbugmy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/ghwfvxwvk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gywxyfgji.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/googiagwr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gjtezsgzn.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gfmhsnmke.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gzxwiuwtw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gntblfihg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gcwcoyhiq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gvapjkwgd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gqfzqfqio.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gmvrxmcpj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gnaabkhqf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gjozsqnnr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gkxhogvvq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/giqivoknv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gllmvrpiu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gygkruohv.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gblufkyqs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gifnjwwhv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gyqbsalfq.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gcntdxyxv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gkkfbtwig.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/glkamyqha.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gfycopnfy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gfqlkjcmc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gsksvdgtv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gbmawpksv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxmflegvi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gzrlkejkc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gddxfbyth.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjvxiodzj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gxypnsxir.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gnlvybjkp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gaowzajho.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gogzwajun.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gwmclusjg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gaaesqkqu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gxzzgskrw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gqseskxas.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/ghhyisjgx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gixltrlbd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/grijyoufp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gxdmpxruw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghcjvgrrt.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/glqlsbrcg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gruwqmfls.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gvhbqfnbd.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gkssxvrfx.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/ghqwwrvrw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gfcwrufoi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/ghlksbppn.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gkbxfvppd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ghdbwivls.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gttgaiomj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gqxuzoxxd.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gcsrhqaae.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gookmhvcq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gbwfrnbnr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gcxjshmys.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gthfsicse.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkgfgpjeq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gkqpowocw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gxcnfutef.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grlyabymw.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gnrcklibz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gdtltjfrm.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gspuwmmdd.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwplhyblm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ghmrlolal.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gphbwqspk.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gbtigxuyq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gqkhusfps.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gatvoihls.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gnkyhrcjo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gksazqqup.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gpuxenyvk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/goslyngom.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gbopihimk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gxwerenio.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/ghctsmnoq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/garopqoxw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/glqnxftlc.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gquqfetgs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gjjbjtcff.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gifzpstyh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gcmjrdbdv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/ghrfvmrve.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gikxbrkbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqtuyephu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gattgcqkq.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/grdbkxnuy.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gjmhmuizm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gszpmnfun.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/guzsogcgc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/giteuexxj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gantmrzle.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gztkdcqww.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/gabqhvhxy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gjsujnyzw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gihscsnsl.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gylleldte.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gguclrmme.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/glbkeimjz.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gyefsykun.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gdnwmeswp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gycihhcxb.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/ggjffbiya.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gjtgpyrvs.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gnztxifpk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gahdurxwm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gqkckjchu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gglprptaa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gowchnibd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gfaegeptd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gcjnqpsky.sHtML


<!-- 参考信息 -->