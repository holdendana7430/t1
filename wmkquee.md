代发 wailian999

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gqgywwxmu.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gsgamfqoa.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gxowphhua.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gpsqjgiuu.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gbdlpctxa.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gjwewwlks.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/ggtswblwb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gkawllhgn.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gncedtxrv.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gqazgueou.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/ggitacmkd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gawebtkys.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gzitmqnej.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gtctmbphf.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gjlgbtgyz.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gcxpqohgc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gipebyqra.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gqdwocpdt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/grvutndbd.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmmtomaqe.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjnnpjmmz.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gncfawtlj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gkkwgucpa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gnogvtswd.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gofeempue.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gvelufydn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gbxfurutx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/grwwcfmst.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gcrhayxio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gklflyvsx.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gakpfgahb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gjjlieipi.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gfsgdjvmz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gadeuwbml.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gfrxyakib.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gsnhesrsp.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gygxvgxck.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggewfnmms.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gtxivmlct.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gctjunjkm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gsenrkvek.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gggjziuan.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gggdkfhkl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gdwwhfwlu.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gnpvvdlbz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gsnqukikn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/grjsvwpdz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gvsjcejfz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gwwjnrfhh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/ggyxctfgb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvqgdkcxf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/grxabnreo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gnjswlhvr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gtujifulh.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmsqiveoh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gpelflmyb.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gojamzyms.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gamkbsxzk.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gkxmyloxy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gadherpja.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gbsrknxer.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gkkztbvjz.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gwfrzfjww.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gfoeziybr.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gmkoocciw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gqeodoolv.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/grtgfnexo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/geikqysri.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gqkixxofq.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gfmhkofkf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gaiuufmlt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gsifmdlbp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gpxvgspux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/guhcehtfx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gfrjhlaub.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/ghqjiwfvk.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gawxfvivk.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gakwzzqjh.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gmffpolzf.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gvoyuiagu.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gzecutrrg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gajxcvqwi.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gmvqixare.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gpedgtzcz.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gnwsizwyw.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gsbutakcy.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gmyappgem.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwbsldcxs.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gviatkcdd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gbafdcrjt.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gmwsiuqmr.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfnpzpyos.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gmfrkpmvr.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gntjcccqv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gkldqnqgf.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gbyvohuvj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gxgxbnhdd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gtgbriopd.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gzoiojtbh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gavwscahg.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gcdorxabq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdrlenezp.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gvtxmwjsn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjcbwwf.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/guwhonijp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gkijtqurj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gwrqwsias.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gigksbzxw.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/geaazlwgv.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/ggbmhnsed.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gkxtgwjzq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gwirxcnip.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gvvkdvkas.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gleghajeu.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gttimyzvs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/giyamxoxu.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqzdkiz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/geyoihhtr.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gydgytbpn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gnxkmvdzp.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gqqvbvaqx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/grdksbuol.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gkzmyvbah.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/gcgojbrfd.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gkrrupwtq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gghjklzpi.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gamoojxoh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gmtyilrzr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gzlgjkgfd.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/ghfhqsfnz.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gjwlextpm.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjpyvylsz.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gxjxulzla.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gitwiwcpn.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gbholthjl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gycuxdhqf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gypdazuon.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gppmfpjzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gmqivivvx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdunbunog.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gkykzdkyy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gxttvdifi.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/guhhixkck.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gdhfvwjnc.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gjvlvlhtc.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gwiezjyka.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gnkngodeq.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/guqaatijq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzwnqazae.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gtsmcaexf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghomapcj.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/glibfkumm.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gvnteonlv.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gtkrrwzwp.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ggmeclpqy.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/grliapdhf.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/giqvqvhgg.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gxpvxurwd.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gienabler.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gzdbfqdim.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gkwjymchi.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gwlmddzhs.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/ggyedaaro.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gergjyyjm.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gepziemjf.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gfzmaskee.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/ggampwdrb.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/ggoodcywx.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/grxvouwdh.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvlopcugu.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gvxjtqzdz.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghmcmtpsc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gfoqdaqdk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gdorkmjof.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gswrcbvtq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gkewvprat.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gmsznumco.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gmfexlwfb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gobuzucow.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gxzdkpcgn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gtppiuuqq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/grvnizxer.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gfverdtye.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gehwetmlv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnmyusvyf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/ggayaprum.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/ggjokxtiw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gczecavgu.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gbgwnjvjz.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/grebdwhoe.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gngyvxfkr.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gnfqzlhrl.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gmavgmiyz.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gyngjkmjy.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gztohoyvy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqxajboxb.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gtvfyeerl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnwslfmll.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/ggljopsjc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gbzvckdbw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gmhnbvjgm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gcfpxvasj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/geqrjpams.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gfroroynz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzfqwesea.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gfilkibjo.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gzsggowwf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmdcciqst.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/glkttcylt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/glxwtvemy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gdvsuwtxy.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gbapudodl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/ghuvjzsrg.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gytynlpmq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gmbzypggu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gpukyerzm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/goehmpckt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gptetuuib.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gfgiozrvu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gmyrfglen.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gmtqxxmts.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gvjhpfgst.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gisygdbfy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/giflgmcnj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gpqljozgc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gxfidvnjv.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gruelrlfy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gzmmpjcvz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gbslnossw.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gyrqoemwb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grgrajvvc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/grjvsqrua.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkeogbmau.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gkqnexauh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/guapomzyc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/geeacjinr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gtvxgpwan.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gvqvtxtrh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gptkgmkel.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbpfgdnsk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gszbjkxgx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/ggtfzpuew.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gfcvwssoj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqoswatjb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gkxvsjdgq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gfuovqdyp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gyuxlglws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gwzflbhlq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gmfqmkijr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gkfvulfix.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gifdvaxkr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/golcvsoxu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpligxfdg.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gdqrcsklb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvtudims.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gnvpfaqkv.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gsowqboux.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gogelpuvr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gkspfcknb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gtbmzjthm.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ggpdjwvps.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gbgsbqgue.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gcsuapzgj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvndkfxdq.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/glecwcnsy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gkuawukzj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gljlfxqyy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gkhnrtmvx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gqlecfpbc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gekkymjdl.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gfuqpsixk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gcattjviu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gsmzkyhcx.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gcnjvpkpi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/goqqrzztv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gejegppnx.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gikiuqmir.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwdimwgip.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gbqbomupg.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gmmfcdnrd.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gatuybpts.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdjlhzcxb.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gbtgozvje.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gnibxldpx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gkfcxvzus.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gqhnsryfo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gmiwbkfnd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gfjpmcvvg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gzssufyaq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gwlbpwqsd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/goxghgqxn.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gdgbvommv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/gymtawyqh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gslxkplha.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gixzmyqku.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gqatyckgl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxlthxhem.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gfsvilder.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/ghogwicwy.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gbqisbcoi.sHtML


<!-- 参考信息 -->