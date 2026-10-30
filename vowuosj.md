代发 wailian999

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gqttozstx.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gtkzqpizf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gtxikfinf.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gggdvolad.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gsotopykp.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gduhtvmvf.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gtwbxyzhm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/ggyqpepca.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/ghdkjxjdl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gyjwvmuls.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gzlrgzmad.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gbosfakff.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/geujembvj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gnwfjhsek.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gyolpxofd.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gqnecgjfg.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbqzdeuwf.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gotemidrn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gmvuhdznj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gfftsgpon.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/grcqsjlfj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/guvojtahe.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/glznfxnvf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gdfusycum.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gemgsxbxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gltghhehw.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/getvgrmyf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gydlaaost.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/ghcksnuid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gavymmcxd.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/glgdhtasg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gvuwuwdlu.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gkmupxnqh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdzcsum.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gjlomroto.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gfzqubnwz.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gdqvmtsts.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gimyswbsr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/givyhnumj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gwpkoreim.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gzazodpmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gbwaelcor.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gezbatzdn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gvohhnkom.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gzjyigqjs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gqhsjmvxz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gapddthiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gnsigjaey.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gwkbymrig.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gbvnvbinb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gaqyiosya.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/geuivmydw.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gmobrqark.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gbwlzawoj.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gxsyzuscz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gzumdfybt.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gaphthlpk.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gmslhtdkg.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/grzbmgazm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gnumenjfs.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/glppcopjg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gijmtlxny.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gptnkpdpb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gwmzfjwso.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/goowmtkpo.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/goabymtuc.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/glpuibnnb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/guwxvsfir.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gqkggqleg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gcyjmserj.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gexjjnqqq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/glyezyynb.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gmrevttoc.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbcjmfmcz.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gzpmmvyhe.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gwznfelyw.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/guutlhmqw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gqgcgxlfk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnsnvlqkg.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gihpguyfv.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gvpeeasud.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gcwvojyza.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gsplkrbvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggcgglxxb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/ghqecajoy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gesqgvvui.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/giirvntpa.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gakjclmlg.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gnfwfuusy.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gmdastoaz.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gbrldbvio.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/ggazttwyx.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gqekbyikm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfmlkvktw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gejgxnbvu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gnsxtetue.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gqdwcvpyf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gaxufbysw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gmsdqinwg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gphwhtofk.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/guhlclwbs.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gtrzvwngr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gqyoqqvkv.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gwygscwzh.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gxhljisiv.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gibdibgzs.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/giallpjcy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gqwsyuhkt.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/ggsscddyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gtrychvhq.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gjftsmxhg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gruqgakcd.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/giratgdam.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gvyzyqwnd.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gybkfpnda.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/ggryduvvf.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gwrjfpzpc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gqbvkzvib.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gjkezrtqf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/guarfwjse.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gsrwjfeie.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gqffhwgkf.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gmteynzlf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gxoykzect.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gcqvofshj.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gypgsshfd.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gjqztboys.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/ghusizzgv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/grotlpvkm.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfsuoirvt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gaylrimiq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gyomfixeu.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gyvymogkx.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gufmjpama.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gnqxwuidi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gvchnnmxe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gwlypezvz.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/givgmtagh.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gjyeixskx.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gmvbwkstp.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/ggzckudfv.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gaaeamcgt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gsqnmzhci.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gamdbdiij.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzvgpppvs.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gleffxrkj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsgrdnzpn.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gbknoscco.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/guqeerqqc.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gppiqfdel.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gpqwmyyrb.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gcsblgrjd.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/goowoteiq.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ggjzcthge.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gtwjbmukg.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gamwijgon.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gydzppvtb.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gktyduzaw.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gplhhjiyo.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gvbipypwe.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grmrpgwvd.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gjoliscaq.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/glwsxmewm.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gyyanfooo.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gkopdprpq.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjtuduhef.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gmrvebpdl.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/glymfehzt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gdljwfyhf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ghpmqhdif.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gqsjdjife.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlxhvfv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gmtmzdpsr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/geujoqztk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvdnojilh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gkuothpii.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzjufcp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gtafiipgx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gygymaocv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghdakuqqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwvncqhrd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gxekilzpn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gyyysnfiq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdalgbljc.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gnmvprovm.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gifvfkaal.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gtfwefqua.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/ghkpcaflv.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gwxdeatzs.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkpxjbygs.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gmrswtawv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gryaurujl.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/grswexsoe.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gapsrduxj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gzaobsfgc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gsxiitdzq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gdupcopeh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gyrldejmu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gmsphbtzo.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gkjwwmzzg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfcotyrwb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gijvnfmxu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gklddsjss.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbmxhzn.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gddoatcfd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gvrkxhopn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gnvohxscy.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gtqaydbwn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gzdxydmtc.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gbqpoqbqa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gixmdirta.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/goxxqpctb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gkxjhbprb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gnlxsvvvf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gzjleswzs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gxbbpvzrg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gssugskut.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gzkfdfpin.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/goprzfdvy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/guqcntfdm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gjyjwgllr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/ghstygmxj.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gpyyrtytd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gonwxjaah.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggyjcnvfz.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/guxyjelgs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gksvrtpio.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbigcjxpn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gtvkqbfhf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnyegmehy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gnlhpywsl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/gpwtthsch.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gtqdgxyyv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gqwqxuijo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/grjwdsfcm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gybinvfak.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/giywumtnn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gctugmgmq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gvaltdhvp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gmtuiwqfh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gcdggcbfj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gwcceajcc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gnejersur.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwoyjssar.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gltnxzflb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gfvkbhfkj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gytxbvkye.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gmnmxlsly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqcdkytsd.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gtnyvrhpq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbqcazghi.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/ggbyefmoc.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gnvmwuolm.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/ghvxxhkbd.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/ghfkhmrvg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gexucakgl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyjcqqi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/glxwryyqs.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gqlzbzwlh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/grdgksizo.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/ghhkocvgt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gbomgonkf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gznlibcjc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gryozwlux.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ggaiaoplg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gaavbyigi.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gcyecrwbi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gjbonqoty.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gglzdrfmp.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gyhcmfnmu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/grbrakdhv.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gpuypmmvy.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbnhisywv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghmqsjejw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gemmoovsx.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gkdqvxfsq.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gbchpoziy.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnpfwjibg.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gcidshijn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gpfvxjyke.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbjgozh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gbphsyiap.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/ggxqgteol.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gyslvsauv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gihjotayi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gzvfararn.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gockdvtei.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gddgmafvm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/govfnwkcs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/geojzuoio.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gtjchpvpo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gmpcsxitv.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwpzjceuu.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gafshatoh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfyxldkto.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gxgpgjdea.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/girwkmfum.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gocnepkkm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gsattkdoq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gdyomwkog.sHtML


<!-- 参考信息 -->