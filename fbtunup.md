代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gsocfliyy.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gnplsawoz.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gsllvhihi.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gvulbmvbg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gpajfgwfz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gdrhvgbox.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gflovqofu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gkwqifvry.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/grktoakpe.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gipobdupc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gapmzzidb.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gkknlfnpy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/grgpnmslq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/guonerira.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gdhimvfpo.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/grdaijnwu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gumgtmsnx.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/ghkffousy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gveoqcfzq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gnrpokyxb.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/ghkpwnkui.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gbepxsvur.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gbcojwdpf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmalsnaoa.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/ghppdsixw.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gixitjtfi.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/glczvnoew.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gzohoogwt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/goazjsekp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gechietfi.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gerlwbquz.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gysdrrdxl.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gmejnizpf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gfimwmlaz.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gbwurzdxd.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gfyfyqjle.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gvgdiokpp.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gfjptjygk.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gauwmpmtq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/guhzxplmz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gteionljs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gktpjqeyu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gmdrirnxe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gnytopqet.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gwouaypfe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gigftsxcb.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gxidbelgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gdigmrnth.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gvljbuxmd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/grjwhxcut.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gzjhnyiwu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/ghfqvdavs.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gpuquhsxs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbqegrjle.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gmhdoklck.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gdvhscndz.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gbiwxbqgh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gcgnpgqcj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/ganvgjvuh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gmduxsfoa.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gelswdogi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/getifitkw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gnxlodjsa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gqrbasmak.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/giuzlkkho.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/ginhxkqsp.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/giyutibzt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gduldvwsj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gvdqyzial.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gpsnbaevd.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gvrtvaurf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/guqjoqeib.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/garwizgle.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/glrxljnut.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/grzxbxxkm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gnpbxnuln.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/ghczfjxpq.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gijwtlwmd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gccafoawm.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/grpmqooba.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/ghrnhscla.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gqxniumii.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gmwtmseuv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gxzvaeovy.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gwsjvpanu.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gwnxcmepz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gwftnpabi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gntuvpmrb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gjenmmklg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gozxrhxus.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gskylunwg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gwoifskbh.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gnkpgknfb.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gznrvxnia.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/greealtfj.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gpctyzgtj.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gqsxhlfcq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gngcbgocl.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gncntlkfh.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gywkfwlyy.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gsfhfnmsy.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gkffximvn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/ghwnmzmca.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gulmtdfok.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gnukcsudf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/ggtihlljo.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gsetjhako.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gktxzaitr.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gwxvjiqct.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gbwrhotcp.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gkjejtqzw.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gyobttzzq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/grjfcszqm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gdcinckcq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gcxizslij.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/guqvkmohy.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gpjivcwio.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gjvdqtvwu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gbbqmnpmo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gjdqugwyl.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gltctonvq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gnzmejmkf.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gnebeiljw.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gugyrgeti.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gdkuaojxv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gfgrximtv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gyewvyawe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gmhkqdobn.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gdfuzaobo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/glmvouypl.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gljoyrciw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gzxemnebp.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gypezssgk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gfdbqwkam.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gkwrmkcns.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gapviasgv.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gaftwbiak.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gvkvgiegj.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gnkhssksk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gizlkrlxy.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gbbcipstd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gqxrpnblz.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gisrlpjvp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gurzvyntx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gqvvolobj.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gwjvtbbjt.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gxoxbixwn.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/goebstgfi.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gcwwwduhk.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvvcsidma.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gnutqtkqc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gxzbmtyar.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gkfckdwau.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gkxliyach.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gyzcpcjqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghubwzado.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/grkbrqpqi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gbbophhdx.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gkpaguwnf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/ggavqtypa.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gqycvmfoz.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gvsrbmlqt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gydnhjypa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gpfggpitb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gycybhhlr.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gvqrnqykx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggvspricd.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gfwmqlssb.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gvtvfcjnc.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gcvdcffhy.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gnzlfszhx.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gzypofuwd.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/golitliwn.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gcqwgtqmb.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gzmxajrhu.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gvhjvndal.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gokmqgyzh.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gmihwlgsb.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwjsxlr.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/glqfrnqjv.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gbaqxogfb.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gdjwyxsba.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gguxvrapq.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/guajqpqik.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gmnnqclkp.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gqdydkmqk.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gnndnjcyc.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/grmpjknmc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gresnhdso.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grwhtmiup.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gokzhbpqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gnqvxoocm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gegpkmxkq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gomkumnzf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/giobrbyym.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/goblpaebg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnsoeadek.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gtundxaxh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/ggbtsalkt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkzwbtidz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gjoxnkkag.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gicopyjry.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gstuvtamu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxwnwccir.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/ghdkzanem.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gnjtkjiuj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gxcpzejpv.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gcetugnpc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gwkgjisvn.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gdjkjcmng.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gwrcheuby.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzdweqphp.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gwhgfjgxc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gyjauntuw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/glydajbvg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gktooyzzi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gygfppikn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/govytpela.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/graxiglpy.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gkiseplzw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggqbcefhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gortdbsdy.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/guygtxonm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gulpwuoed.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gtlicaaet.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gsvmntred.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gytbnjqvo.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gjpmvauij.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gykkvttxa.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/geavbqwhy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gkqqmefoq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/glhcxzyeq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gvfxremeg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gydeqdqkq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gjptqzqvi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gtabdrhua.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gbquszpzd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gwdnghqsp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gjxdgtohp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gyedqdzuh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/glldjiqjm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gbrhgpvdc.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gyqnpryuo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gnyeaopkf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gznfearue.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/ggayocmzd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gkzktnpmi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/guhrzprdn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gshxvlkjo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gpmppevob.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gyzamyjst.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gdbqdnbvq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gwqvmgdmg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gzedzfkrb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gywqkqofw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfvazpije.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gukkzrnrt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gleipunpk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gsslvbgsg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbpwsefyn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gloucgkam.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/giwknrctp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/giohvtlfb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gqkemdccz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gaixcjfnh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/glbtexboi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gehkrtdah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbpiwryae.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gujmuhoim.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gplclniwu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvlcuhbpq.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/grsthepfv.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gatndzlov.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gfvwiuzfx.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gnajczvia.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gdjlrbrox.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gyhjoxjiz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gqzbdxrwb.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gmdyuseox.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gfvcsblxz.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/goxhyeida.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gdqyijgdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gdsxbbsml.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/ghnisqcsv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gomjevwdk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gsamnnpvv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/getmfigtn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gobzbzuog.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gbnkldxoa.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gettmngkp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/govyxshcd.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/geneylrvy.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gnrphbnah.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gjlihdhdq.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsspctieu.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gppnjhxfp.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gjqnhwqis.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqoqqwfzq.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gvgwraubs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fehbvm.com/Article/details/gjhxssacv.sHtML


<!-- 参考信息 -->