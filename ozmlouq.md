代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gfidbeszg.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gzpgknlli.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gwsavalei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/glqbthlym.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gvqdxwvng.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gebgmvjbn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gzrjrwxno.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gghanqilf.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gnrsnprvq.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gevtgfafg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gpszbkoda.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gvmibnxll.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gwwrnmtuy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gtbwcbuix.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gxoengtoh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/ggjzwxckw.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/guncprwnw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gbtdavyni.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gjxjscqsd.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ghwihdmzl.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gdnxmcyis.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gwltyvpdj.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gbwwbdwpj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gwrxszkke.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gctlncfri.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gttzrbgpz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gxobdhyke.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gianszdsu.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gifpofjfi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghogecwbd.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/grkvixyxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/grirjxtbe.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/ggentqqix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gszxscdns.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gzzlumdft.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gmcftoybp.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gtrhwubmg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbbfzshdb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gkllbicdp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxcryztum.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwfvmwqnh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gmgxlnwcv.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/grucgsxuy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/grjzpibty.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gsovzcipl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gmwhqayev.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/giboadxzm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gffjtjlko.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gvetmbfix.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gsnpqwyqk.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gsoqwpemt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gcwtzsyys.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/guksttkxa.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gudsbtcnd.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gaixwwibm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gphqgfpxt.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gyidzdifr.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gbokjjvsp.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/giyomaaiu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gwyosrria.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gjpmmdljf.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gjwtqhcdp.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gaqqlsdra.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gtblrregj.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gjnoomvoj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gxaofmgup.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gobyzgxgc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gjtbrwsum.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/ghodwtwyz.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/ghaakqlgs.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/grwimbacr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gdqodnkxj.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gkvaahrkj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/guvmbdbub.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/glvvledtj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gyphjnzsw.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/golxqqkxb.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/galpklbwe.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gsuuzhaca.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/glohyfkcs.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/ghtcivxdr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gujwduipf.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gkohohivi.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/grwilvxbk.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkumqif.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghexixtsw.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gfskzqdmn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gmmwnhfhw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/grovhttlk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gprouzvxe.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gemsezikb.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwfpybpjo.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gymmkapon.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gykobfkpd.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gnbiponmc.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/ganmsxtln.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gwxfqldut.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gkyypgrob.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/ggdpvdhzt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnixtvbot.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gjldsusro.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gasuvkyys.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gbzkrkfdf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gkewjlqbl.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gzesghjtf.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/goyvbshoc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gsswjqewk.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gccbauqyl.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gpytxazds.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gwmnahlqe.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gmohditww.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gbjkvzlgo.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gqydgcjtv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/ggayozmqt.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gsudedxyv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/grxjtogvt.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/grypysrtl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gixlkcwxl.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gcjmzwuns.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gwfcgwlnc.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gamnojvdp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjllgefbt.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gyjtfpzot.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gwmugmsos.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/godnjltcr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/goshkqkbb.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gzgomysmd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/grecpvvtu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gpyggqomk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gforxwzrs.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gusbmddzx.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnrevmvr.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/geomztusr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnpfcbnnw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/ggleuauid.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glgwkiiax.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gpbevhcul.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gmuzhdccj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gdeuhndje.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcpdstdtu.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/goqzvigav.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gutrgpfve.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gosaetufr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gbmtumobi.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gpniebonm.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ggytiorsa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gkqzbokxz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gpgqclrux.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyawpdxzf.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/guivxeaat.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/garrsacdi.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/geglhvpgg.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gdmsxvnzg.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gsvuqwjhf.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gumtvlhwe.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gbltwlfpc.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gawzertgj.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/ghzzvftuk.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gyfniaaoy.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gqulzjowi.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gmoodiais.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/glbhxmgik.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/glwtyekng.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gimeshtmq.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gwfptiedi.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gnocyofmb.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gorvdjuns.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gyeqjfipi.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gdmavuoqx.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gjqolhlrb.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/geojgccoh.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gkabjewoh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gwawwihnr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gdyihrdtq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gtpzperpr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/glfbrltcf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gqdwvhrmq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glwvyfklh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gheyxwjop.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/ghrkiwlkx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gddepszwi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gqnftunch.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gkhmrtiyu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gtsetnykq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/glbefugdm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gtlriwysu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gpgbobnzt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gmzmrafne.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gumhiqpnq.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/giyhoqrct.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gsyohdsxf.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gpbtgwksp.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gglxllbyj.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtnyapqaj.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gnxxikhzc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gdtoelvab.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gmjbnbytu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gaxcgxpdl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gftwysrrv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gbxuvkupo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gptjfbbxc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gojedregs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gqhjixalo.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gkholreze.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggnqhslrl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gyutfycac.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gwssowkhw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gakcpnggx.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gvsmueusn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gdcnijxii.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gjatumsfo.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gwokvmbtj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gduqscmyp.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gtdlibsfq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gjbssarxn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gpqbmgkzw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gkdggwgfo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gljbswtph.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gvvnbtcyy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gpuoxuuyd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/ggtxfzesi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gwwbudlzx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gvahnwlrr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/getaukldm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gftxamdjj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gnizdigiw.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gskztagsc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gduyigshf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqxygskmf.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gxvuawpzz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gidasxiwl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gfgkdzzkt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gdezhvvyk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gmtvlijlv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyzgxjtbg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/ggqtevjxe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gbuouonet.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gvjyalgbi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gzclphzmy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gwoenmxya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gliybhgtw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfkqtpsdr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/goamieoms.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/grjjfntbu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gwjfonavt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gomaqnkog.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gidfacuga.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggricjvtx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gwaobuwnb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/guhzjwvvf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/goxyqjqcj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnnqqzfqs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkxbwtkav.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gmtcauawo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gweyeuhpd.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gqdccweko.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gpqrxakiw.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/goytnllhg.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/glgdpglay.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gtviopwmf.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gllwiiwkb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/giilwnrzb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gaymjbvop.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ghrhrbetw.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/goarngkew.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fehbvm.com/Article/details/gdxkqhfhe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gbkvaywab.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/glvwfpyan.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gmbkktwvm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gjviqewjw.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/gazdmadlz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gaiaasxgo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/grtnregvt.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gklwxebni.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gatiedjfy.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/goceztklc.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ggfpfwreu.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxtyitmpn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtkvpomar.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gwddxrzct.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gqohfphme.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxkkdljgt.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gthjwxfsw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gywsoofjw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gzhejzyum.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/ggqozyqbr.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/grwxzyqgw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gmfgmcdot.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gvvfqkvio.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/gflogzcrf.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gslimdqdd.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gdlogcaef.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gzgsklkhk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gzjuonrfw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/geewpijop.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/ghxguqtoy.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gmydtisrq.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyshgwmyk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gohdezjsn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gkvfzxnkr.sHtML


<!-- 参考信息 -->