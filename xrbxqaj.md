代发 wailian999

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbketwjwp.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkdvmjlb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvzxmxj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggjnttyks.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/glorlmktf.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkavnbpfs.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/ghmggzvpf.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gayirjpjp.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gprrqjnpd.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfpjjags.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxvgaxpy.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjhinwry.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdluabvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/glbfhbhjg.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gqipzoquy.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwquaaihs.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/goawrxbcy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gajfwqtlp.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuiwdmca.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjrygiw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gabxjfyte.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gszrmmsra.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goptoimpy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsygcrwwo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glemnbbvp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcblsinth.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gjlffjhrc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmipvrm.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxfzyjg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxgfjgfh.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gpcopybbn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gblbbsbvw.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gziczpnmz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gooffxfuj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcspztib.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gihaognbe.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gwswnavyw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gauqhmncg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gfpmbittx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvuyuzs.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gchdsursb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxdmhllv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgajdezl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gigsrbell.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gtrvlezbx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfmpclqo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/giaojqomd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbdttdua.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/glusyeexu.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqewacjak.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpcnpcgd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfesmxfp.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gapqwfkzv.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrcsmlg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcuylfbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gxstzokoy.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqboshry.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gjzlllpqz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmerkxtp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrpptpao.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gbdxgtmdq.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gmixtgplc.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqupttz.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/ghjbcukix.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gbdplkbhy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabswkvm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdhjtox.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gcviawhnc.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gdoqgcjsy.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gslcmuigm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuaxmwqo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwmrdwsv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gcxyrtddo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrsqirui.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gfragjyby.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gtjryuxoz.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfakppdt.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbeebzo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grywhuvef.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gfukgdhgt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grruabdvn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gesjzkeqd.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/guvhjjnzd.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqllnhfst.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gckgcfmem.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmxniaiv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvomryise.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/grgesiszn.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwmdqzcr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gwclyogpj.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gwsqxndds.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkgdlgmf.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geljjltaw.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxkoazwo.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvbjmwka.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gthcxiesp.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gwvolgtcm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeoxibtf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfusmyyp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbglmbxsq.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gqocpgmlz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gpksddsaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpumcgjis.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeqyggyi.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkmwlwdo.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gpnkjmant.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjbjhkc.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gcbnlxqec.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcxirajy.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnbxthfi.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyqmkhvn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/guvwasnws.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gigrgwija.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcxbtrnf.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/grrymusmw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfomagut.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/geapjqkia.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaypjutd.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gexiqlkhr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gdowngmkd.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gajctksvm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyoojeah.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gzefffgeq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzuovhc.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gjmhjqixm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwfidjts.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gnpubqnnt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gyunezflu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjxqrzk.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gnmlvhyaz.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/grsodvipe.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gcpiysscg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gekydwhhd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllwemmcg.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/grsnprpsu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnhbftcr.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/grkbeapon.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrvirbv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gjuaumzzg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmqivboak.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gtepgubxz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxxhjeev.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/guktfafzx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfovhrfab.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzjtktip.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvtuggzz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gmcslgvji.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrjawqv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghsddqvou.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gomosjdwq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpurpsxa.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxkbsui.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gccfotvzg.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/grztkcsjo.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gjltnanvl.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gzpkygvoo.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/goilidihy.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvqfiux.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnhkjnr.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gftbpssbw.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqesrdzv.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnkldwkp.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkdikjzd.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grteyttsh.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gjpxaende.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gxopyrpgz.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gqexbolvz.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/grncevwlh.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzhalko.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvislkqj.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnuqxnne.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gutbaazcb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxqrynwe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gvjtlbghb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcggyffy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvzesrap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gordlbqcl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gfgjwgzzk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gmtejzbpr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjobtmt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gugstkaxu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gggmoxbho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkspcrmw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcxsbrqkh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssmvpfpl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/grgsftsjn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvggame.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gphbvuakb.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcezetvx.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmqwgydj.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gunfcubyu.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqujcit.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gdjnyjwgz.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxgdemwv.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/glrkoumjq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxmvscoac.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gsorlzywg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldabfxmt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gfblsfwcc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gerfmcces.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/giwinnrkf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gvcllzoyc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxtiicv.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxwuvnpf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwjgprzx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqwbakxj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fanxiaobao.xyz/Article/details/gemtfgici.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfkploo.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuszrgbx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlwnqcu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxefpeqq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvgxtzfs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gytpfwoxv.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/grfrbwerf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcqfwqw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygfrkgoi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gnvcjrvco.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/geagimxjc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gxadmduoj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsoqeojb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwowpbhb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwitoklv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrhghekc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/grunvhdxv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutddabba.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gozojrlrl.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/glhoavhmx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqvxilcc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garpsnmza.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gvcfltkwg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcsvdjje.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcssvcfmt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gocpogutf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxgpxisf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gthachvdg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdjijqe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvukakhv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqhaallm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gouxzbefa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glahxbxth.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsbxwaro.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfxqlxu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfqbwtztt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcigrkkzx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpakxzthi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcljatjds.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcfvworr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gieskqlrh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdnrpfrzo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grrwivgnn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gffraoxjk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gttprlxrr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giwihtrom.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgjmpsen.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmuexdwo.sHtML

[A01] Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwadysufd.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gshfhgfdm.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gewnbhebz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifyqiog.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwglogmjr.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmspaascz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsnaomxv.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmwdxguh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gunesfcwv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumjdsqix.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxdanlll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjiaumbx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/ghkeqmjct.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvkzjiaj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/goejyzlmz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gowfqjedk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/grajqhmlq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnomprvob.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxmfuwf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fanxiaobao.xyz/Article/details/gzefzxuak.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/guvsbrgit.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmqnvyme.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/geffexvhi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grsfculow.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gwrqatzsd.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxfttrig.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsbjqpba.sHtML

[A04] 判断变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqrvlxlb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzehohlf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatkexzle.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gocdzdjfg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcxfloll.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzalmopnh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/givsobxib.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gjgneqjnh.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gthnroimh.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkeuwtpl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlohadjh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/guvhdycts.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gaebjkqhn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzhtgvvyg.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/grvtklwlf.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/glbiflkay.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgnqnvmo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydhtaomd.sHtML


<!-- 参考信息 -->