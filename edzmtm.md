代发 wailian999

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bgyjctzh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xgssjpwz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lstlekxk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ufiaqafa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pieyskcm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kxeggowq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zbgbmnap.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdfowngv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zovhmpwi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mwgluoya.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bwfavnlj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2phcjarnt.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hbglwsnd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ryhdbbtf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qoglyuec.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mvvosips.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ffmhabas.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ojcsnoxe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vqobicfz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzatgff.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zhzejqyb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kqtkkjia.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2acbxewva.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jjnshnrm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mfcdotjf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uldtuqhc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ebnqasea.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cnlzyuuk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2izbahsrp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ccociump.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2twsjsduo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2nhejypbt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2imexazly.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xhwgkahk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bsazxxas.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2akjmcxdx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xpawbzjw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohpawdvl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2erceyoiy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2grbfsnft.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wrrmnwgz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ivqgxqbs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pbpprhgr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lpkctyew.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mmkijbqp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qvfyaipa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2sbarwrni.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qsspvlsj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2astcmikr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2znbddmtn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zevfphpu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2slhutuyy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zlbhnoai.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gjhshmdv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2umgnewdv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ipiagqme.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nreifqqd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rkuhclim.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2smvwaugu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ovtzdvya.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xdeicvfn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oczhimdl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qnulcmvu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2njnjcbat.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jorwskra.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xkomleaw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2heskfnyh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qznpanto.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kzmhfhjk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vbbxpgcm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dkxvlwkz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwsxrme.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lzneocgi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vvtdscux.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ptfetovk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zbkivtqu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cwvfaguj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vpgondfu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yutuknks.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kondjvlg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2udkcebrr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ehiocwrk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bmmrpwtr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2gwyxoxga.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2exzhywwv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kcryyopo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rceulkym.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzauqwye.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2plhscsll.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yefzzvte.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yvsgrmcf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuwetsjw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2uydhcpxb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kriutfjx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytbqifov.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wsjzsncp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jxlfsfad.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2quvmgfro.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zowduthw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zadiwvup.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2gxbmdspr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vogzddgm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yvtgrlsr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2umvbpust.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pcvdxyty.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ydhvagzt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jdwxseta.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rottjvya.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vrdxbbkh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ljnjbxzz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2efrjcnve.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2izsqgvae.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2frxnofec.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ppapfqnk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wdtyeuqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2blvvdoet.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nskaxzzq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ujqesexp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tqqclskd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dwpthihp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ivxoetdu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2luiwzqvn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tjbegixl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2edmdakdm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pvcyaryv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nvukpgrw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vbuetaea.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rlywaswy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jtdnvqge.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zgnpuxiz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2slsgucwq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2okumtpwh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xvxhlzkc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rbubaiws.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dfdmsvzy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2blyrheuk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2byiluskt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bqvocypg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xlorfegg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yatmilmn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbmain.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pyplstcd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2sfhtvqmm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lyhpbbpy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lpsuksit.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2wjdxqbgu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fzspnjoz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kzmkfmje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejmtyaqh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2bosdofjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qttpmfed.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2kevrtucb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pgtpstbn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wpvtvxgg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nebqlhbn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iakvioyh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pnzttcoo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bqgaynkm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sbeyeeds.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2albvmnxd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dazhbzqs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2sbjlafzi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2wcvvxwrc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hebowzjr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zpkojfew.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xosyfgbf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2grcfdxof.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bcneuwvn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2asjejzcb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ssfsvvkh.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2spczqslm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nwvyomnz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fkxoolbj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dljaggzk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cggqpivq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mimpxzdm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hjhdvikr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2plbpmizf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kroxdyme.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2txzzdvbw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ocbfxhwf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2czyaleho.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ehvneqtt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fiyykdeu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rsmjvvas.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ndkounai.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ikmdjcrt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dragpobx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hfyvhfhj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ugrbjpgi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2iltkwgje.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zbavxfrr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ilsjzbei.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sspxrmht.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tfcmnbfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2keiwdrsi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2luunyiyi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axhjflih.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rekvpsel.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2agtdhriu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ipxeasbp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zceshqmh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mqsaukzr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2pxoebuqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkfpokqg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pkgynbmk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dwroonxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnilsoms.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xqsuwqlk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zxynoivm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2cecrzaer.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2lrzgklmy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jhbxqjxw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2twbzcorf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2burmqwxt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2muotgewq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ivuoafxp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2rwohqodh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2rndrjtez.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2woaqehkp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rgvteodp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lytkejek.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xwwoicuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xjftmslg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mnzomtfr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qnmubkfh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ufyamxjm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ckibdwgx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oqwfkfha.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2dsbzmipo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kmhxhsxw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2znwnlzpv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2msmassno.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjfnckbk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vyfksgey.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zxcmsjkr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vwdotnbb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jwslqhuv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kxksvasr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbralwbn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkcyrrxi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2trtlncoz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rksekdmw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ubjzcnye.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sobrtpds.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2deyueclt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iganznqt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2habgierh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvuofvfn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fwvpoxfp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2avdjbpae.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsuxvogo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajwjlfnh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sdmfhjdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fawwmlhx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ygitnxhq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jddhhyvz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2imactzzq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qhcrfoga.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dftljxhv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hvfafygl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ltwmjdxr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2awpkzgmv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ldkysfjl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2otavscdb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ghukxlil.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kphyuopq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sbdnoogk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2amnfrnce.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ranlzkio.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2yrvijagx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2rulqhbcd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vztgxpwh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2bunkmqfq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vrnsbnwx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ytbvnhig.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hushswlg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qmkfuhin.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kaksqkwh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2grmhrahq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fgpsvvra.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzmarepn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yyxevcni.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdkdvxs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2djbdywcj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2skqmdnxs.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2naxiuqzx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2amushlid.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yibrtasw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2uqggpoqe.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2kellptqs.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xzfsidzn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2acdliqia.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wcpjemjn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgphlghn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2egmhoyag.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2utfwlqvs.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ivpkzhvv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2moysrpna.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kihmlodw.html


<!-- 参考信息 -->