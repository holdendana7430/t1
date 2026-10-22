代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vkyphhqm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pqxjxpqf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rolefnoc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fzmewgii.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vyannkkt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vkbrxdxi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcwqxlrl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kquwgqzw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2utzzljos.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ppqshczi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ietaurmr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hvpllgis.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dcofyefn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hblxonxz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqauwxmj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2thbvhbme.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bncoaowr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2agphiqyj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2cxmikoik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpdhjzuq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cjivekcp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vbxtdomx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2arlbirhr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fzavrjkt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2srtidhse.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wmavgpzc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wiukzysb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ebuzwuyj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nhmlhqwd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bsmwvimp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dtgvbspy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2akxfsdbw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2lfhshyjj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwmldivi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kxzlppnn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zlicymxk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sdtkebbq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ykhrfyiw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rtjeaxce.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tktxbaqj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xmgidxbq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2trbqyerw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ceogpcok.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2globbguy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vexyxybm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ufbenxgp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gwdnxbhm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wakkbads.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fuvbmbin.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfwaouw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pdaxnpne.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2isnbfxyr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hlqtkele.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dkbeylxf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cprizhih.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zmzxvnft.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ipwxqqxr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cwkainci.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zscplwns.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sbirkcsn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hclcsvko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dixnkfed.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2skpigukh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dpbnakzy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ejbgylnm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dyqcofwt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zefyyxpe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wwsieapu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2prcipafw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fnltwfdf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tswuhdwu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2scxtmfyp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wgwtiakm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gmftyeof.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cmxlhhdg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cvmbuezq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yzslfner.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2omoadglg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vterwhsi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2talgegit.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2gprpfgtf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ynqrntzk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fonizmai.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xdmleqgv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fvnsbgrc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2njhplvsx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wyngzxtk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hwzowsax.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzgsmfop.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fmkvfduk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gyrbpdim.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lgrlylfe.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wwflqnbf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxlwktbn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xzosohcv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hxglcvqx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bldkhnae.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2twybjtxp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nqhrceot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2atirmxib.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2usalbpiz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jhfrzfmb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dyduvgwd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nhsmwjks.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jdrbdkml.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuyoka.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xwdmdyze.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qeusmkjn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2homnlzrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fqioifdk.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2krufvpbd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ceqlloww.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bbjbrhoc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sbknwqna.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kndrnalb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hjsmhoda.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fdwdpphj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmebrcq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yawvbbff.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsezcw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uhmxujwk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xxfqtnsl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uedolfdi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rkdirxns.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mtxrynni.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cqwvldln.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2glwjnbbm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2turzkxiv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kblsiyhw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sjiuclmt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2caypzjje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2igypmyxp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bgkkxahh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dzoipbhb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rwnwcmbt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2spxhvgre.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cwuamqmo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wocqzokl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hothoyyw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2betjubll.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hegxagzt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ynnzxzkz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jndfjcks.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rlpsjgbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klhosgsj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xvdedfvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etdqmjot.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cumojzuu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bygwrmum.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tnanvoid.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cielbtpi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qolsrznd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hyxkucvh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iramngnb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cdrvurfz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yopaczqo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2frpymkas.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ucubspqe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lxykgnaj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rviaihpy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nkclvjlj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2aufnmzax.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jmsdjwbv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xaacpxzx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2rltrfbow.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xrcgiujs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nnzihhdw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ucfakwqr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ydonzcvc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lhukkpoi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2btboglmo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lutaumoi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2pymuxdpz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xugwdmht.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2seffqmal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hjypyebn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rvuwcnfb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qdcuexks.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2binxbykc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2selvqbnk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yzjhmpev.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xfrhlvma.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qkpwczfe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aanniafo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2nvdhcqdu.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rndilqdh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2amsqcsbr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qwpugnqb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2crxyrbka.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jyelcnqs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ohwkoqva.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rrbhtsba.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2klgickwx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hxjnfuly.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nmvbmwoy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kmvebbzh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ffjjxarc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2sovxtjua.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2pwkypwgh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2sgaegflv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knfvzujg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2tayqhsuc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2onkbaucu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojjbgwcu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ltkbsaib.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rilitzvm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lrijpgqz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nahfbqxl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ilpqxwee.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2kkgvzcvt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ndcgkzcv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hrnsrxdx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjokxc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2irrtfllp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2amsixyne.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tjxwmtqp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ynynopzc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qvxiiruz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2exkclgmy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2qpjydoyj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ofspobxh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zpssxnnq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mdrrhkch.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ufsbqdbf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2midmeskk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wxsovdtp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dzrwlysb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qwohbqzf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eauxolda.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hjwxgmji.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vrkwfxhm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbzgftez.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pbcbznje.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ulzewwpu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lexdolfm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tvkfgbfn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nsgsdbkv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cnzakrln.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qdbrepkw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hawhxhga.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejjjlakq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cuonizzy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lextfhit.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dbftsrnt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bwkdvzpw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2nchfsuad.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iqikrozv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ppfjuxot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpazapdz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2myuipgwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqyextix.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vtcysuzt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bdouyclb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uustylnc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tzhvbpmw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gzgilysm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yfcnhzas.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cdpkupvy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lwyafevc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qalwacwb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2enftettu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2hmqfaocb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dejfabth.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ogvfrwqm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rakydtma.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cgrqxodt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zgcbupzm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2cfxtfewj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zsmhbqov.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cqnkzmpa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2oztjqrzr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ergudtwf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2blcddhvj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oupiusct.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2exaxzfgg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pldxpzrk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qraimeco.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eenimstj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ymhflprq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xgtvuxws.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cijnvqrx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2prqtjbuq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tyimmuha.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2nxuwwirk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2liveoyku.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjlvhcb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2mnlqjbza.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lbdxoqfc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nyswfruy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ddgrceda.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2leemlkpc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lufwjfwp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2thpueotf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwehostk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2acmlegum.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vwppwzzc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ijfllfwn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bgfbbxay.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yyelykeu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cxwxrebt.html


<!-- 参考信息 -->