代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guzcbewyz.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwzhnrx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxfhinmu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghanhlcaj.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gpedpychl.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gtfpuocsx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/guzknvnbz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgxsqilh.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gevqkfinq.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gfrhqigng.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gicslqfrq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaycpwih.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/golfpxwff.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzcamke.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyqeune.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlqmkymr.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gdffgjwdw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gejzjglgo.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzyrvyesa.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grnurwlug.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwlfzpii.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbycoliis.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/ghqpqcpzr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyjfpkpl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghopgzccv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhwzwgfp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gmafhatcb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhfhfri.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gyouypiqm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycefaqnv.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gltgxkllp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gwntgcnhn.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gxmfaivaa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcwvhjbk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyaewuizi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnmyrtb.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gmyftjiyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvtjtbic.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqaecfhn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gezbzxkin.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/grlsdgxmp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjwkewxn.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcubkhydz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gliymaozd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gwfbnoghz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gmieucvhi.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoruebty.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gwovjgdws.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gazjcbkod.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gondpxeqt.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/govaybsqx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gfxvodnkf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphkvjbns.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjotyom.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glkpcmpzv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gppffmmfv.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gtjvtwima.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gfedhwaqu.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gyjgfnslo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmjyweam.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gjavblbtq.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/glaczboql.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrxnvvnq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gkslnukis.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjpzcikk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbyuqglc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gkxzhnhmg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbyrcak.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gkghdaghe.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnoshyzp.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyybiefbi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/garfpstie.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzmbyvwj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gomfdmlhm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gngqruyrr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutdoejag.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gppuxxzvq.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/glewqfqdu.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/geshzptwr.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gfnnbkjfa.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghizpsqmh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gkakmdwph.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gjlhmzodo.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubkhnagy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczobzyva.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkipqvbth.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyscogsb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjtsigr.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gunqwlghk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmjtzgxj.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gqcifvhhn.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gvijppwro.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjkpjkbsi.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/geekfjqyu.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnbsoblqd.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gqkvzpcbs.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxvqfzzy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gisdfohje.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gvovurlxl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfshabjwq.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gbvxxksxi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdcqdej.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhxmgakb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisgawjlq.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckclsws.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhcqiype.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/ggozfxxgy.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxhtudvr.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/goydrgkny.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gurgikgjw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljdrqazm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gelhxgplw.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gaibhbphk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gsmuimktu.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gyinojwlb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyxhyft.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gnnefpbfe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpwrsaft.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybtwjdis.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gvvbolaqr.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjycjoxv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzgnyyq.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjniwvnkw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkflspshe.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktkgfnaa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzczvarh.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulwlfvks.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gkwkkogst.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdrskogm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqyxbqpo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnrovqfo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbrplzz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/golvbzcqk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/glvsxowto.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/giabdsxbf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/ggztttdhw.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gudvlzdzz.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gygrqyhpo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fanxiaobao.xyz/Article/details/gaxoeqmqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glrvhapfo.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvprvfri.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gyajiqnjy.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gqywndxip.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gockiwkrv.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/grnydjxae.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gsbwvevle.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gerwpvmas.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gjydisjxc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ginvdvaae.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvkvqrao.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyfjyooe.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gkpkqzfzx.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcnndlw.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/goklikpsc.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevmwrbrh.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gipheqvsd.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gwhbexhyh.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblwfncvj.sHtML

Ruby ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvbmpnf.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gsqlruzah.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gbmhjbwym.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gglfpfrjr.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqiwsyvl.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsuxtszr.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gecvofgyh.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gxirkmszl.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkpgcvbw.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gcqidfktq.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gekaibksk.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/giwunwkdo.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjindlo.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyajoier.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gajidntst.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsonbei.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gpfpjiepa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/givhqvltx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/giwrbjwmv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjqaiex.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwphoxffm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gffkgsfyb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqneuqbyl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhsohbkj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gzwvzgqun.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvljyiem.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/giklczkmn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsawxoij.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjkuyhpa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gttoheyra.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdppizia.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gzgxeerty.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gtyeincta.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwypavh.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gvzwihchz.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gbymgfuza.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gngbmzxrr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gtseqbsto.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/guelotmdl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gbqmjqwvp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gdotbqmjz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkfhhksd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxjllznk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gykhrybha.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gigffamue.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gvxrugolr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/govmeitpa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gudbmdqxt.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/glthvisqt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtdspyqil.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gofepkfap.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbfunkgf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwikduuk.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/grtvxtyio.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/girjxeaek.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/grnrgbdhp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gujbpubyh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/gmoavzast.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/giwckpfhg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkzjxgam.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/gfhjnlbak.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gimqjgych.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/giifaqjbx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctqvgkx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fanxiaobao.xyz/Article/details/gtpgjaevd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddmryrtg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzywgphsy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/grmefpitv.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjkgzfr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/geowocmoz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gyicpofig.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorfmcifa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpqqngvp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdnorgwt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gltigycyl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxgrhpvqd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghhggzqum.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfytzamh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabrxalq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gucrdqhpf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbddgnbhw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gisustktu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxscfcpxv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoentncy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gsyryosho.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzcszdzv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutakgavg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/guwjkompc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gupigzhok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gregywons.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjdtrff.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gocnnunte.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/grmirqbwk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glrzlhqsw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grtgrxmdy.sHtML

A. 基础语法与类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuqhbay.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glwipvpdk.sHtML

[A01] Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzgfxfts.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwumjzbz.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fanxiaobao.xyz/Article/details/gqbofyoab.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fanxiaobao.xyz/Article/details/ghrrppxmo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gckbbukes.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfcfvpyk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gljgjkgoe.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdphojbgt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwwstoj.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/geoquvjnm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fanxiaobao.xyz/Article/details/goqmjijll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcqbhdy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvjokkn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmchuqavf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaklmketd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckqkujec.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fanxiaobao.xyz/Article/details/gszqcnwab.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoonoxxj.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxccojqp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fanxiaobao.xyz/Article/details/gvhssdknv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbszdrwya.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxelgbvt.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gegyxoilk.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruxymjlp.sHtML

Go:   const PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/grqbclpiw.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gahfvysnw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmuvfzeh.sHtML

[A04] 判断变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclteaglv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdovfqbr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqzknrsd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gpawmuphv.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvwxobhk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fanxiaobao.xyz/Article/details/gcvsjfbpw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmhtrdxj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/guishbhmc.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fanxiaobao.xyz/Article/details/gqbpvvsfk.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoqndwsl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnrrjdlb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhrsutr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsximvhco.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghbfgzamj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiqlbuuq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gosfcipjn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauzmrnkp.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxszenvhi.sHtML


<!-- 参考信息 -->