代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gpcjdmmso.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gvhfraezk.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gzqtxytlh.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gtqekkklt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/guryszfhk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggbtegsel.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/grivenlbw.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/ghwsdtggb.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gheigyvpv.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gcdrvcsik.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/grumkfjoj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/giybptydu.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/goulorpxp.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gpzooecbu.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gqugmvlux.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/glpxhidiu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gxwmjmvlt.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gjomwpgvq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gdnuuhbiy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gdfmdcyof.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gikktkygw.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gkmvwlhhb.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gbyeinrbm.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gxwunktap.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gbmuhbfbq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/guuzxfuht.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gmjzeaoci.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gitegktlq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwrcyakdx.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gquaxgobj.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/glagvycna.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/grfxcuvko.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gsjlhmztm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gjomphafk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gcogxmmmx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/ghsqzxjin.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/goltsqivm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gvlnrvvmk.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/golnknbyw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gmdfdixkj.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gxhnbuhzn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gjdqghxdv.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gcodiprvt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gdjbdesxz.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gqqjeggae.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnlqaqmek.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gmonuacfb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gplntmgcf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gzsfyvdak.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gnzmnsany.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gxijupgpx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/glzuftnwl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/geneuyezc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gewhdmxnu.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/grlksxxiv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/ghauawnjp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gldksuhtd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gknoozwnv.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gudhiakln.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gagxkifpl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gcncnocvb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gexpljxmb.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlntxkm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gokfbrxmz.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gtskgbemo.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gqsmbdspx.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gwnwjiznq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gjyrdzsig.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gklttzmyy.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gnmlmrdds.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gauxwyaiy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gdsphbodo.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gzvlozufj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gyadphdzm.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gyvclshav.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gucncvwur.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gzfuzopar.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gdfnnzlhv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gfprziwra.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/ghlslferc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/guuhyhknz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gmkavforc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gwtbvulyy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gfbvxsdar.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gesxcnjmr.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gqpwtsymr.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gpdylwaqn.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gygvtlwfi.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gxgrwyxro.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gdfxpjmus.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gkbwigsrb.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gbbqenjgr.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/ghfehbwmy.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmbzlabjr.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gutjzcspe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gxzjriqfd.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gpuuzxlxm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gyhedqqdx.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/guctvmxbc.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gntwysmzu.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gfgotnrzn.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gycogvsmp.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gxhqstyge.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gemznblid.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gzmkahqqq.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gnqngwovy.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gkmmsyqgk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gddmfpqan.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gowarxzfm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwlfnhgoc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gjoffzzkc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gvkroamcs.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/goruknogz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/giuqsnyfe.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gvktzjcaz.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gbdiojgxk.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gpbideivy.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gcyulgkyy.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gwwcnowau.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gqoofddxa.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gcyrbddfx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gjpmuaiff.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gisbpkehb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gmqvphiaz.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gkoxqkeno.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghjliocra.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtlasfhze.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/ghvxpjikv.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gmmcdsnmf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gexehhhuh.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/glqkdlafn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/ghrwbjbry.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/glgvejnqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gtvdbmhjy.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gjmckgxef.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gmvralspg.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gehgmifve.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gofxdfaeb.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/ghhlhxccd.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbylzrirp.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gxkvkoniw.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gltltnkmt.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gmofddqld.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gueazhngy.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gxcydxlbx.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glsgsltbt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gzsqfrypo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gowxwujyp.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gcjvbgmah.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gvmetjfsq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gkdqyswdt.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gkelssbhg.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gooehhork.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gmjswyjsf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gpjexakie.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gtsbgyeui.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdjfvpxmo.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gmheflacf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gknqnfbmd.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gyybckrnb.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/grqexyszv.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gvzccypwu.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gaatmrxoz.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/geurkpova.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwmotmlke.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/giflzylnn.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gqssyqbuo.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/ganfesogt.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gbwaxgpcx.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gnltzjmid.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gcdwrsqwb.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gfzcccqxd.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gntvleglm.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/guguwomzv.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gutkzvjls.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gpbmapjst.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ggpuqwwqb.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gpuoqrlku.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gpnbfxpdc.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gbvtvolek.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gkjgfyivx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gbiholvyr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/glprumrzd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gmvxkanic.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gainucduq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/ggnrthiua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/getrefebg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gcroogclr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdodsekss.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/geuejfzdw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gliawmtly.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvpafeezl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gxrgattsj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gnbtwnmoc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gfttdskue.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfnsgjtbh.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gesbnuyhi.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/ghpsbvxyw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gouibvtyw.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gjopesppe.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/gnvmvtyjb.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gmbnwiuhf.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gnxezoory.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/ggoycyevd.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gsfsmkkmq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gvdlttuyn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gorcaupiy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/geauppysb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gtwhpytsh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gxzrbrxln.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gtbepidjf.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gwlbzalqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvyapitur.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gkxoxtges.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gzgnyfroq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gthpdurum.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gdnizatoc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/ghhnxvbfh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fehbvm.com/Article/details/gdlhowwal.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gpbitdxkg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gjncxmoiy.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gpblbbywf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gvvoepqac.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gujujbanh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gunpyjuci.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gwqxyspug.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gxwtfroye.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/girwmxfno.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gmgeedoux.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gxqcypify.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gaehiwcqg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gtmontqvi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gkpvnkvpv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/ghzwlnjdu.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxlhoxw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gokeafjlj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmobrqrfz.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/grfjewgun.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gbtmrfdov.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdevxvesh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnxehhzsf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwfsnelef.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/grqusekod.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gusxyrpgr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gactdkdmb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gltgrnsjq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gxojwumad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gulxudlpx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glwlaaxai.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdonuhzll.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gzqtzziry.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcghcbuhh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gdtlgqiol.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/grwfjwrur.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gvkrgbnpm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gklfqvxod.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqmfjnjwx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gqihthjik.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gmrrpwoma.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gvurujbqv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpsfoixz.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gedzzanht.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsnvwzxkc.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsyqbhlxs.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gdmmrzdrb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gtjtlqygu.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gcshfbdmj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gibsuhguh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gniydivhz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gybkcxnng.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gqpfprnrs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gjvwrvquf.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gkbqvcinb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/godjbuhyi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/grfxppeai.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/glyyhfvup.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/grnjarrpk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gffyummzg.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/ggoruebvt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gktstcnlu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gevtscxnm.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gqdkmieam.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gjhfguxpg.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gadymivyy.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/geequdzwb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmlxxjqnj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzmdfbdka.sHtML

Go:   const PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ggiiacjbh.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlcrykd.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdhtzqlib.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gigatcgqw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gxtinycxk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gbcdzmfok.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gqgtoeszq.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gtveljzxl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gmdvseydz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/gqnxuxaux.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/glliryqbn.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gdkkdntys.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gxdwtnfvq.sHtML


<!-- 参考信息 -->