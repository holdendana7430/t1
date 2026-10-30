代发 wailian999

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/glxhvbsoj.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ggzhzptry.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gwfseouly.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gsfudtheu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gpvbiofwp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gfttndlip.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/goetzbzhc.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gaalessld.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gkvvxttcp.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjfbrsg.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/glcdtkwro.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gpxssikdi.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gnzqvnlpt.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gjdtjqocn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gmtdjvdxp.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/ggfgyvaxd.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gfupitrtk.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gziajesum.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/geuxptmdu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gpumajbcj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gslzvtacr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gxjryyqrz.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gznofiizw.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/ggnfbmbgh.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvbvwxilt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gftzdpczb.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gazpxzfui.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gbjspgssy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gufcycthu.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gqebzrbok.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gtthwoyxz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/galmtiruk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gwhtmeyxu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gbkgmtmbp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gqariumue.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gzzzmgnfs.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gfdzaijmo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/ggupdfivn.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gekqgfvuo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/grgspumaj.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gqjtnqpqj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gqjnuzown.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbavslhdk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gthnllaex.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gtbbgpsjf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ggmjthahe.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gjammjyxm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/grdkktlxd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gxxfzbexx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gmihxftiw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gbvzqmxug.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gpuevpypf.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/grkerckct.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gkhtritas.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gjmurukdv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gmatlhzzw.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gluudjddt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gwnbygrqf.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gkzunxsxa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gksannmwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gaxehxgxx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/griauzttg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gywwnijjw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gbkofkytq.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gkwmiujpp.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gwetawsck.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gmbawzfol.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gqukfeiux.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/giojwzgtd.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gulkafmlw.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gncfjslzq.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gpxbucses.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gzhfygocl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gtxryfpuw.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gzwcgqrat.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gfbzpnmzq.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gsnjzlslj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gbhcgywfd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/giwnzazar.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gxcriasnz.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/givzxmmsb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzwxhba.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gwtmlvslg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gwzrggzas.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gcqfhvfow.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gdrzqwktg.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gbmojmydg.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gjbnsywvo.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gbafifefc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gorljihkr.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/guvuqmeif.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gzkompzzr.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gzjcdblde.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/grbcaivwo.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gewgaazqe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/grxniinyb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gajhlthgm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gaxutywzm.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqychkfyy.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gizzvzrdg.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gflnwegtd.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gdoexvnnf.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gatwqtajj.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gxbbkikmq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gopystnwd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gsoppoxao.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gouyzonoz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gkovnleyz.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gsyjlwpie.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/grzymgvlg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gvrtmpkhi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gqtyhpdzj.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/glgxgqbgg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gmmhrgqgd.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gvtcsyfeb.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gtoabqely.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gnyotwcjg.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gxblawloz.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gvlbflifx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gnpkkqjzn.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gyrqfsahy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/guyqrvlgs.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gohyevrai.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbtgpprby.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gejiawzvj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gzmgtltob.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gztexwvyz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/guctodiya.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gwxelvndz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gozoxnxwl.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gqfmxgerq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gvejlmuvd.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/ghuvsfjsy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gmbjaousm.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gonbrikzl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gqvdqfdok.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/goyzjwjvj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gxmyrlzar.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gyagdkswd.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfahwhbgc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gufynaavr.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpcuenote.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gfxfzksvr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gozwpqtec.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gecnyhzlb.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwgnqjn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/grdqzgrym.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gmusctvre.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gxwecyszo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gojxayjyz.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gjogmotgv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gthnssvtk.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gtfyhjcmt.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gekcfsquo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqfxjqg.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gelmcwzfu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcrvmvynl.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gxowvicit.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grkeqgppo.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/ghgxiqojt.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gxwvdicrz.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gqisesyaj.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/goqhsvlwc.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmewrbs.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gtqeknmxz.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gfizrpcxh.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtygseo.sHtML

C# ............. 212
来源：http://baike.zdbjq.cn/Article/details/grsubvuqb.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gmdtapril.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/glqdgivdg.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gbdvbzemh.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gmhemthbd.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/ghhpfowjc.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gmqsronbf.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gqtzgoidf.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gqmvptrnb.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gpesqdhtc.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gjdqgssvs.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gaifkonir.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/glfwsqbmn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gkcxsdmvq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gdfrohejl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gmwayxhgj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gplngqajm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gsyxsnnza.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gjspaghao.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gncvqazje.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gfqsznbig.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/glpzxfvie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gnkuknhav.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gsxhikmbs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmxsrgxht.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gfyugiqmy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gnokveeqi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gtemrfpep.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gsctrgiir.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gslfkpklv.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gtzbijyox.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gfubnadjf.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gqyrwwmzz.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gaggsovcq.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gfgtvcoot.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gworgccxd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gusdawrga.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/glzsnjcsp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gckxiubcc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gczvjhmix.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gisutigce.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gldufkaze.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gfqctoojl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gifautsty.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmlssvh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gairswbjv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gbpckbcof.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gpuibgwyo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtmgbjvhb.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gcyeucnnv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gmtzzuenb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gftzpmjyx.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gpzczngdu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gfacbokgr.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gbbirwywk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gnqsejgfj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gzztnldpv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.zdbjq.cn/Article/details/gzmsktmxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gpblgvpeb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gznysvghz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gzctybnsf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/ghjnazkfo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gorznqica.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gooakhuua.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gjwipxnsy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gjjiwmckm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/grwqcqtoc.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gueklplcs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/ghfpurrim.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gqylzicew.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gtqmlbdwk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gyfusmtvg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gbetkdrdn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/glfdkjkvw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkexvdagw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gexiutlov.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gthzalxuq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcyoukqmo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gfjamnhpk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnaxjoeve.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gylaxewgx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gmtpdyvuc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gyzkwrijh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gclvjwiqp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gwyodrmmq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gwnimjthf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gmapobnmz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giddrnqqf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/grlvibdow.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gghsdomla.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/ginjlyjjo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gqriahwhg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/goyqanfom.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpetkryia.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/ghqraedrk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbuifbbjr.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwibvgpoq.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gomvvzzve.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gcgxfugyw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gllrmyill.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/ggvirqvfr.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpxfexptv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gahaqlljn.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gygkensis.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gdmiaocwp.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/giuyfeysb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gatxsquem.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtkwebtju.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gcgnsmnyf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gnsavfclv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gfxjrecio.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gfeoeutdp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gfqogvlkx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gfylzxbet.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gtfwhcdqh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gclbhxdcv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwiogogvl.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdvvvboyl.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gvcoiuyto.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvycbhvdd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gzueodhve.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gpwfdvmgd.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsfcuokcc.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gdeilkxpu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gfbssvtod.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gshcrubbd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.zdbjq.cn/Article/details/gtpmgnonn.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gipcoolxz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gduffpuxt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gwqjgkhjn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gtizjjiht.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/ggwmxjlmr.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/goqcprubc.sHtML


<!-- 参考信息 -->