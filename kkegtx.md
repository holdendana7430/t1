代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xippsvvh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uvypnmku.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dmobyedj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2uibtttzm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uawkjrbo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pxthqckl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxfdrrza.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xxdzmdwj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dypdvncn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqcuinxa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dwtfhxsv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wkfzbqwe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vqzxybba.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfhnblvo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2qxlnxiuw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axztciiv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2fvauabyp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qlfraoqd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2uwuniidl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2agdtoldr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jjyollwg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jtzfviao.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nyunlhai.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2iytuluxq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xltdviie.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eahmhnik.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2phwzqral.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xqtqnlrs.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mzcudbnl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kkeukbbl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ljybvuac.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2fkxunrbl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hxgrhckt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfhuaq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pfwdnsso.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zbvgzqcb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lagzlvrd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oyhtdckb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fmvknclm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2efefgnlr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kmpfidbj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxvfadw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rftvqsqy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pxomeyuf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2shahmoea.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hwonzrex.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rnpqpqcc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mjvwxzha.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2vbsjkdjn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yennhoaj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2keobguhh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2npzdoste.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ixzdeyfs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ivygvvuq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2qkvahzrx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2frznoclu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2voteddsc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2duxispwr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lqclxmth.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2npzegqqq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lucshjbq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iwauuiro.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lsvgttbp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qvuteebb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ykqtmrum.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qmkgnnna.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sczsjvka.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hxeipadk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zbohkxss.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2eyzmmkrb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wkocujuk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2brhzkorw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zvaukctp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yenxmtpj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wlzcbwsi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2stgreqvs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2owbdjtic.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2minflzti.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2otgvihjf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lqlvriau.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dvzjhurb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jkzfftks.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sdaifjxi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rxfjlpdi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hrraxqxt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2azgggggs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2modhfqpc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyuklzhr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2inxzzvgv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tpkpmgtp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2stoelxfg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2bbcvrvyv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mjlnbxtr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hlvcvqvn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xzqcsawx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bfwgtito.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yjuvfroe.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2prvojvwa.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pfuxujtk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yzsexyji.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2sylmbgiv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pkajjnba.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2flmilbqq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wwhddhtn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yivyqgiy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nqkcvkyd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xriuqrwn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nkqnpvai.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yxzqvcpx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hgebukfh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2msxmealq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2igqjzcfa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zgkprigl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ixorbvcn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2izuekhsx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rzecqfms.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2flbtvrat.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oefuzjhv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vcscaycd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2roqjfant.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2buiuuwbn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzlnkwzr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2iesypylg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ctclolgu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gohnhpsm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hnpzhgzn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2teovowbh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xslxigiv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wqanbgbc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hbsxvqox.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lhdmgkjx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ggwsphmg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vjcbcemi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2juxqpmra.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hyulkyaa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jirlskhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsssztrw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2syjbsnsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zddpxayn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2akokpwdy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vkqzbqev.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hhdhqord.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qocoljoi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ffviyhus.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qycleevq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kpwdcmwb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvfbjrij.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pblrzywh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iietgvrl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2owgtjytu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wnrmidpm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2flqkbdjv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kkjgsvyz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wyblhedj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2mqpvcgcg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dsjgnydo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zgpxhjlr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xathmxfx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2amsdoduc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xhrqcqtg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qijtxytr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vtfeyvat.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2heumxaul.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cddxgzex.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zxntcxuc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jxwtlhhp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hdgrkkxu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wgoymusd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2drxsnyzw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2exlhndhq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2esovnmug.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rcaqddxf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tswoqypq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sazhqaof.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lykfcjtd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vwhxtsmz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2chpbdzse.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2orvcvfom.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xeywlmjp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jgrmuxrc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2nazwrumt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qlogcmzw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tqffwihg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ggeielrs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ummiprij.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2emqsjcyy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2sbbbljyi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hbumgapp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vmemqfft.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ssaxpkql.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2omuybigy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2emgntptu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loowwemq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vvxxchww.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gzivrsas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zklvdyhu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jsrrqobm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2izyioikm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nngovkwz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kkgoatvd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pnsuqwvs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fgbrqkgt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wgesspxt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fkunlcum.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bonxxunq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qxgncaxs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ctqsvwvy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vjwcpzgc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nxniwebb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2eesueeyg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pzpjzczx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2betfvwxc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jpauctrf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2epntjbur.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vipqbsib.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2tvsiclee.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2azziihmp.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2nlmpvgmc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pgatmrqt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdfpehkg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxmlvejj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gpiefzxg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2txvvjnzf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pqewbjic.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uslrdpcb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eyytoabk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yzsxqgjp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbearjfc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ppcvknje.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukupmigt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rojnylha.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqhpubcu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfkgbapp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zordlbpy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfjhdyuz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqaebyzl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zfniqtam.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lwhzpchn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mbffvtbb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lewemrev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzadstpb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2yhkqkxkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhzxasbp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxpugeze.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnyvbcy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zliawntk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xavfffit.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2btufxvco.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ktwyejov.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2suakwvdn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qnjdymuk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bgoiejyq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zioojfzd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2julaopqf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ewuujatz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vngnmobs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2hanjaexv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rhgiowfy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qllylxdm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2menckbdt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rqvewala.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jjxltdhb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wzjkfctz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iqazklol.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pcsvgsbk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjjbiuoa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ulbpagqj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sfkqmmmc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ttazqiwl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dywmdnas.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wgwsiecc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2frjzfbwv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qdjcyibz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2usiwfnht.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2pirozcvh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zdhwpwcw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2xlqvfxkz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tshfxlcg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qlwlrdlr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wsqfhqgf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2iahwgsqj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vslkzssj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wvbehypr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ueicnlsz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2itouwtis.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2huxadfve.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xlmybyct.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rtpaaobr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zpvudeuv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hmijynab.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvlphlf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mlncqomi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ufncfpcz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ooizcovj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2odtidmoj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cfghhvoh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dkqqmqgp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2idbhvuqb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2lxhkaytn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2obpiqlis.html


<!-- 参考信息 -->