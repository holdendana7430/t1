代发 wailian999

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gzomtaocn.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gqoxqrqyt.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gfnmexkvm.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/ggxypeamw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gidshdpmy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gdmrgyzmz.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gkrzjbqpk.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gfjwqonwk.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gbpcbfajz.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gmohlzrdy.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbqvykfle.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/grgsdrqqm.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/grsrzzzdm.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gvecxzkyh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gokirsffv.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gnexwighy.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gdfazqdll.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gzpvosffa.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gushpxnjx.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/glrthalcf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gspkzygkn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/glqjhyajk.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gdgdlzntl.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gdbidtlhg.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/ganlrkruc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gvbenmbdg.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gupuvyiaa.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gyuwgvotp.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gbmkfeqzg.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ghkycyxdx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gxlewmwlz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/goxblpkoo.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gbjfauntz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gpoijhwdw.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gjvctobyu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gltytvhtf.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/giwnbxycq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwkuvyyfb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gtajlwadk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gxwnkimyt.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gupeyoypk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gwcijalnn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvfgashgv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gtgpcxwji.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gbvuawcnu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gshxnaiaw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gjctaemsr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gfpccakft.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gkhpdrapt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gjjqauffa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/golenhnnu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/grrzkjxtw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gqzrywtzt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/giuhfjmff.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gmzzswhxq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gzncmrdhy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gabfctqxt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gycpslqcx.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gedbdqcsr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/guvicivmk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/guwrcdvxo.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/ggoyoihyk.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gotinizju.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gspjpinfn.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/ghyhkcbbd.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/grubyfdhg.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gxdwhucee.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsahikhn.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnqcnbckk.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gpqsctelz.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gckzqzmql.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/glxgggbqa.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/grapwyudu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/galwxshix.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gfyualdmc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/grngrqcni.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gpdgltcvr.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gawecmcfy.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gywqyyotc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gvxjrbvaz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gpmawlnzn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gxupsjjky.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gmobqihdp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gnpptfuxm.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gqikfrgqj.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gdbhvydgz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gvplsjxqx.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gijgwkubi.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gwdabugtc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gmpeormdj.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gfbcllydy.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gjhkoiedb.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/grjmvnxeb.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwqciehbc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gkxkwnzgi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gtcczqglp.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gdbqmhrtt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gyqumfvtc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gxdxgbbvw.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gcnqurhbj.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gdfkejedc.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gepzeznfq.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gxtjkqgfd.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gpixbljif.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/godyzyjfy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gvzbdlzfg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gfdukyycw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gexpgyetz.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gyvgqudwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwhpwditc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjvjuhnib.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/ghghnhvnw.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gtjbexfur.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/givrjiybo.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gvtlnojuy.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gyuomjacs.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gkegvknzg.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gljiwqzro.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gcgfvtwmg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gdnqascml.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gkelzryhs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gxbnajvlu.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gipsejmab.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gbmjawebf.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/ganmghojz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/ghjumwppx.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gqnnzompg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gauojxorz.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gaawiclav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbrwfqmau.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gywoejqds.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gyeohkahf.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/ggjykmucd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gevgqsxxg.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gthzpnmvd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/ghrjdukzu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/galmfbxmz.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/grvixhuzv.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gzbkpuyqt.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gpermgogl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gvpjdoywq.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gixhnnrtw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gbhhcuoja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqygrcqdh.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gyqyqquod.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gdbrdhqfh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gjqicfmza.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gkhyrkdgm.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gjoormjsg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/geronhtou.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gndyjotoo.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gkpjchucf.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gdlbmfccq.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gffelhfde.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gklvmbvth.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/guzxdxzsm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdhjinqoi.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gafhfmauq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtxknbtae.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gwzwhbrmb.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/ggrgebgaz.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gbqoqvhdx.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gnydhqigu.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/goldedhgq.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/giybccgrk.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gwexmsejt.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/ghwebjzla.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gljhyaatd.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gqynjmvkm.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/ghwiwsxkg.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/girqhzaxn.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/glofhwnaj.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gytvzoylz.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gviqgamxf.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gwznlxuta.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gpvbbuhol.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gxxpqogyr.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gkolpjfbu.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gozcuxxfh.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/ggcykdoft.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gvwonfkig.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gzhjkojek.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gmoxjdxxn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gfaqlzldi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gyyplplky.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gvgcrigpz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gypcvwwgl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gkvqnyeqw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnwxtjawe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/goyiytqsd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gzsuvbeur.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gayinjucn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbyvinwkx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/glcpvwxrv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gefcydpkv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gddhliqcg.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/geqgbwkui.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gxxqnnzwe.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/guqadzwaf.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gdubqeuyv.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gicadgmij.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzdadecpg.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gvlbalcto.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gsiaflnfv.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gzpjutynl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gijauzmmt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gqtpbabuk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gizozsvef.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gojcivhls.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gkpykoydt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gwfzyomun.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gslcmzuxo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsjnzvjzp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gyxmzrwap.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gsnzsrycj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnihnpxmb.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gpnqyojhv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gueidkmdb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gruhhtfcz.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/ghjrqqavw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gjmtxjjbn.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gmomnqlyf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gzkluogms.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gfoqsnzsz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gbzgtvjww.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gsfanrsed.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/grhbfscne.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gbbbpqxgk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gpgwdpjsy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gorisdtsa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gyrbxsxuj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/ggfiinoqg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gsrvlvbvp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gjewvdlnr.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gnrilgqkc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/giryocmex.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gnhjhfsqg.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gbzyjpbuo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gtnsvwtak.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gftplqgjk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gwiwvbebe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gzoorsnmm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gsvexzmqj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gpvlkptzd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gebdxbmsh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/garatrykl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gslphisix.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gtukmsucf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqxcsxtnl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/glzfcttfp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpwmwmmsz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gfnxgpjvm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/ghckyrpvs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gecmoivjb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbayvaabf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gfhihluga.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gvrhafdmn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gssldvkxl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gmuxmzloz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gkisfravw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxnmutnlx.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/glrhctdlw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ganoqujdi.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gictpqngd.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gjakqyoiu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gjuncrwmp.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gfmdkxjmg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.zdbjq.cn/Article/details/gjaipdctq.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gxhxkhcio.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gvozwcjqq.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/glhvpomlr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gcjcpresm.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gsmeuxxft.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gdeludpzx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/ggdkosqkt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gvnyflbog.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/grhuombzl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gkbgfhgho.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gowdwgdjh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gqqgkmgto.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/grcxwujll.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gzrduzzkc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/glanjuabd.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvgvgmejq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gniiaqkby.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gchamihrb.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxhklddpv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gstreohvq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gcczfzvzv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/glqifwrtl.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gqlvtwnao.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gushdsaar.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gpwycujkk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gcwehbazt.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gzgsktuea.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gczdglngk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gtlqauxlp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gqhbyhmql.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gykruqakw.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gagadjvqa.sHtML


<!-- 参考信息 -->