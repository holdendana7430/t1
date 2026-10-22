代发 wailian999

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hmjdupjb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bfvipblb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tlhfvvjt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frnairyp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2axlkniup.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qevsaeoj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bazlicvc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oewvcwwt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xeuakrpj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jwrasbws.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mbeaqgcr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2peffdium.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bhscgrlx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gmincuhc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zcvjxsqn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nbirtiqx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xwvjgulm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ntmxvtuj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rlwqahqm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zeeniciq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zdbfjlmr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tkbjkgkq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2afxffukq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xopauduv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2grjiwotq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gpjcanhb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hsuigqmu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bxuxyweb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cqbjwjzl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mldcrgbx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2idhjxdar.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2divwxbrk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tqpvaqtt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xjpwoqly.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uihclius.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yfkzwsou.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2knibzxwe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wkiteynu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lmquhzji.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wyqdojvn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hvvtqxbu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cafkmjgd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2aidsawxa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cxuseldt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vbsjvrcm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pvtvnkig.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zcmgswvw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2payesuln.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iubkqoph.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2odouirwp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wglaeaxl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2siyeocxy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2uvuqmvdx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bjbimpyd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2npralzye.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rueudyqr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2avbcefbu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wygfwvtn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jkbbsxta.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zdukucuu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xrkzimsq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ycfcmchu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2eoriytou.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lhzdbwvy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nwjjpjou.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2oedkzazx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hpwqhuhn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vtyibikw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zijvovyi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xooxyizo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hwxndvsb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mbtboiqt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hsyzrbjr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cjiboxnw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dpcvezcx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ukbgrygs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cxxzpxrz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2olrkjdpj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zdnobmhx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2snshbfbk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2etwjqcvq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bjncabim.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xajxhwfx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuniivgx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sriqyqaz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xchhjsgo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2szmkvkhc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yssqjrle.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2epmwbnvw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2eehewbsc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqvikmwr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zymibktt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wgfwlmht.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2apgczjlt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2evyzgkdj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zppuqaaw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2crftwksx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bbfbwbba.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dgqkrcxx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pygemsxf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bndxdofh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mgdpwsqb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kvvtftdb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fopwngfu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ykpjgtpi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pphnglhj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2oyfqalod.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sdhtdyrt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2phzotpqm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nccygfvu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ykksbans.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hglvakfo.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jsqazkvb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dgvkpakg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dsoyfmwf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jccydyvo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2auljlbat.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2olgebwpu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zhfqtqfw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2avlhvqzf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fkmfkvrx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ggvupnbm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sdzpzzzx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tohyciny.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hshahzxt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mebywosh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2przzrzhs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hxrtxnkh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wienvroz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vnniotgu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fprrpyoy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zozzxhuk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ruljaznc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vaktmrdr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gjcpqugf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2rrwlosjw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pwvmazbf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ienprnnk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lrgytdtd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ccgwwqoc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zpjqvoym.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lhkliiaq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fqdtcitw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vsajyvcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oejawlrx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wopdaugc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioszjdyn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jkgfkfqj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nuwszifh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lllnkrfc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nsebcvmy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nfgmubjn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rjihqerg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mihxxmof.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lvjcpdol.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pfqwkgsi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2drkknxhb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ebovfwkc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uxcrclds.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2lcxszuwk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jpjdeanz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2zphnkibr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjszfmoa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ltssyrcn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjnicbvi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rwbzvxlc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ooireedc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kvtosyei.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wkczxtnm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2chliahwq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xxhhihwx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qmianasa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nptmfpln.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dwptyjzz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jwyawsie.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zwdmbynr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uhifmfcj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vbqwexti.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cnymtygw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lsjlqzly.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nmivwawr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qatjkybf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2awluzovj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yzuvlluo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2chnzjtch.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kdcmytzk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tvfbkpae.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bbvsirxu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bepyrykw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qprzaqmd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uhlfhbkj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2waxxwvbc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jstoiguv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xcbnzznj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2omlaxqxc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lanpkpsv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2heryzqpz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fudnqeal.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wrdjesha.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xpwlwmqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oorwyczi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2buphxyuq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2jsvvycru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdrfvzxf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kxbgupmy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vmkdacku.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pepgrqlr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ktthyzzs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2wanapgyj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hbamxbui.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xwnwyqtq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mhsggxtm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wsktyefy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vmfecoad.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2naubrinc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2miaeqmll.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jkycxpme.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xugidpnk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mbgkohff.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2soamrnxb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2vorghwng.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2igvhuahu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2blhvdomx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rnzxykng.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iuaspmut.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ewxuhdtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2olirtxwj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2tnesefwg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qzmrvbnb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rdtxcfrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czmzvxuf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2gdgmeily.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ivvujtpu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oarhxecj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ercnfupb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wincfuir.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pbikjseg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qgcypzsp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snqfjgqt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gfbxgkvd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rmpdyqht.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jyglnfdx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbkucbar.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrijywli.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2plyfkkhv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2uqqhgxyn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kfzinped.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2czctbzqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaghrmny.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lswbeucf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cccoigzk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ogxpgfaf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2oeilqrzz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2arwfubqd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zvhtwxyb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2iubhxarr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qrxppmwu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2smpjarbv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fpfdktkl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nytltvyf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2iivablhj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ykerglza.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mfvtdswb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aebjtskr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cdzmgmmg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rijkuuvs.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2upqrcwfg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2trnztjgt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gncuukmv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ibskvdiv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ejbwmfby.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lyhiiqan.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oiiqrawu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qilmxogs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bpymysqm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fdcobatl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ayagjkzx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pehbgjiw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fcadzprr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hwsrxetl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ghaamxod.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vpxgfchq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sksbwxjj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mgrykxyp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jistwcjh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2hrwelfrw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2txrpbrjd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xgrkkfgx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2cxrgzmow.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ylpslsak.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cmtabfjn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nqutbzrj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vyrouevo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bpowihon.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bokkaoon.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ceinhjvq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wokrevwd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ventfdhr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmrvnz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2defddvtg.html


<!-- 参考信息 -->