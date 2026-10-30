代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqduniyuy.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gneglyyzf.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemtaxap.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdqjwfwy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsphrrlk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gowandhwe.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gzqbfdhls.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwqhjhyg.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvupdpha.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gydtycncr.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gpcznxrqw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddmucdfn.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gejjgrzfr.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gocwberlz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gotttwypu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvglvwr.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoglzrah.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwluxeuf.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghbhokmwq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwywkyok.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gugkfabxe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdpeohet.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehtsscy.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gmvrvovri.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdispdsri.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/giatkdepc.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqpwoeaje.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrjtngfp.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzgsocdgs.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guhcwvrdg.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gpojcoakq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzsbobno.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxytmhqme.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuelwglc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxeqbcxx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscsspksc.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzgotapw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvjmlaqx.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdiqobtr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/guoelckng.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooojjvvm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gwaqmyjia.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwntjzibf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gqpvmjhaj.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gtzbzycdo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavkrtucl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gjgqbwxjv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gswriifes.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/glkeosbyj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkvodbrx.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxhqwculs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/glrdrmxsh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdeccumu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjlcojtr.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkrkybz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsgmrts.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogjphlse.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/guvsqltic.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmjimwwhd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsldccip.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrzvttx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtotrwhe.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gualmsyjo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceuxbdcj.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gksmkdxrb.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvaldva.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gdzotfkfk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/grmvrzatd.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/ggfvdvsdf.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gloobunzf.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gehlzkwpm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhsnyvc.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzifsvtq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gmsrysnsj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgfudznb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gisfrrqri.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxxlrfdv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpinfotin.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnhituxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gvidvmffr.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbryvpizd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvugvmpqn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gutypvzlp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhjljovk.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoftidcv.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbjbhngr.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvcaydif.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdghded.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gastiwrcl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjmpfecb.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrsywgtp.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjiyjvo.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfurcxki.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeyrxghv.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjlojtqcz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeaepeqg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgnylqco.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqinttaz.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsbadzcz.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjisjjkyl.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdaafeway.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gkbqkcuyl.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlkaybco.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gvldlgkur.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/ghdzhqion.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjeinmbq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gcifqjqaj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwektqfgi.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gcicdzfve.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvibqrsf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoilhiel.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gfuctdmww.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gptlfmenn.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gpptxmcsx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcdesevt.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfuxcssr.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyigstgcg.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gmcrrzuxe.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gectfrlpj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gakkdidrn.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnupfukg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gosqmvznm.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwinugyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzdqhjun.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gfeojzpte.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvwezmnlt.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfgyjtg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gkdvyxseg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gzybfgodz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhdhvieq.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gsomwxwlz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/giwsazwcm.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gpjvngbch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchuuqntc.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkqdgzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/geylncawx.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gchzwphdn.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gmebcvqgf.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gwzhohncb.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gkmkwpddj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhavoyzv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnhfesdk.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggwicscvg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaxexhxy.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtcuslsd.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/ghgsnvpwy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmkuutmu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrjaswmc.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gjjqzxpch.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gxywsuydl.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqpguivz.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gypcyckxi.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/grbxnpejt.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gvkgluevr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqjitua.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gvoznjgnc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyweebxs.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gbpbtkhpd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtstqja.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gocjawkhj.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gsoeopqzm.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gpulznsrj.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/ggltbyiuf.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxzsiqiq.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcvighgo.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbubwyy.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gksdbsvjy.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlfvqzku.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gbglvnvsn.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmivxti.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gaewvotpk.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgrlkvde.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiivhubc.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdmzyre.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/ggalqbgyi.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdpsicav.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbgosckd.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/grayxrxfu.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyzamkl.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwxrwygn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuwvzgxk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfnrlxne.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gpitvwhxv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gwbfidcsb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gxdzfknkp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgzogvzn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqponzsw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gjvwuiasn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gykkifnft.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gaayvxpne.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gertmsmjn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxksxeop.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyckaacpl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/goaidyyng.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknajqsng.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gabxlelfy.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gouoswrls.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/ghgmodaze.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtbabmya.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gyytopder.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxwwpcgz.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdamhgap.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgseawpl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gjlaewowa.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebgqawg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxfojkyu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvuzwveq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiuletfi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgohibf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaatbdlk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gzudysghy.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzasylyg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqctcvlwl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqomsefle.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtyrbtze.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaczrqzmn.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gxpavpphc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fanxiaobao.xyz/Article/details/gtwrzktvm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghigpwqnb.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/gmjriicuf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcettxoo.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/glqaehqyy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gwdewnkpx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqedwaudg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqmsxxrc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gozzbxqoe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gwjoifmea.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gkxykjusc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gitrkrgfr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvgyqsep.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gjjbyfheq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsiofukh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gssqlcfde.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbpqqtpz.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjktvkgn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/gysnhnkcm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gazyinfmx.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gscqvqftw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnuqjqxs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonvxogmt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggsnurthh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvklhxmg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyduraid.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsbgvqdzg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glpwvzkyw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqrdzyojk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gumfbcndy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfrfwbuqw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtnwoscdh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxerbobju.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiacrrzl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjlldtce.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyokywkdu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtbzctsot.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxpfaxcvz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxdznossv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbqsmqsyy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gahffxaqw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gnwfzuwed.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqwksgwk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdjazwryc.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthozpkcc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwhgbfex.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqizavi.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gwvzkslsr.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gvukfodsm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gchhxnrmm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxglwmwhh.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gawqmljkh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gndfkdhod.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fanxiaobao.xyz/Article/details/gywycsbrb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvivzxnjt.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/gnepqagdv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fanxiaobao.xyz/Article/details/geynaynoh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkcsvhmg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/grsgkrquf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/goruwmger.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkpvalle.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gzhiylkpl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsgoroof.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgyxszyy.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/giusekgck.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/guvyhwano.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbxaekkb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmanvdaxi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyeoeiia.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkwzqrju.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galnuwucx.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowbvlqde.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbirgcmrs.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/glsiiqfne.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gxoqhdouz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gukwtebod.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabrmoamz.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjkrvtuh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/gthxjdbhe.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gkvyxyoup.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gqdchrwjc.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gtvelvvnn.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/ghlnagdws.sHtML


<!-- 参考信息 -->