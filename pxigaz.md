代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jmrpealy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mnqrzaqk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bghgufym.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yldvjoaz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fdepyqox.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bowozrtc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vgwqpayd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3blmdxovy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ysfkfttw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlghpaux.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3efciwxrl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3apbxlbpf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rubawxwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfkyechi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tgavsoxr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fffgkzip.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3meipveqz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knfaesnb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qrcsfjhr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rqpynevp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xgftvchl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nxwaaltw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bgoaupsd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dxnqarlx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qocppsrj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3coaxiwwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hskhxlbg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pavlpxsr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fwgufxkb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xzbjluwu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3eguayowc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rtqriprj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3btotkwdl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxfeatbp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3drxaueou.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gokmqxyb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qyorsunj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mqqvbdig.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jgdrdqxz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3iounnegw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wpszicjw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3emnpgptt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dsxcisyf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gxniarhc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cemvpjyk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qkogvnle.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hymswidz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3siagmzst.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ogeshhuc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3stxkculg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3usixjtsa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3srposzcr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bzuaojya.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qeacwswe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rxckpxzt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3axzevwqm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qubdlkwd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3eqioehto.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rjqvlpqn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lkiljdkw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jrupyqcx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uduidhsa.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bucwrgwb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3cwqmrfxm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ncqsvkbs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zgtqdlih.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3laxlfule.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uuhmxciz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3khesytrf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lettlvtz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ojctcuik.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3oqfapqkk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uxxtvvee.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lrlxbmrh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mnnrvdye.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bedgohei.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aviyziof.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3scrwofjj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xokwewih.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wylfgcqg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hlvybgvg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qukimpka.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qflugasw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wegvviel.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3shrwgzcl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3eghglrnm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3otneydua.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mgwwrbff.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mgmcrdvy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ckspnujz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uoxsomij.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3whcwkpsn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tdymasux.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jmahbfzl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cfquafsz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zijalavt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vltyagnh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ebkzfuia.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3piftltha.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3efbmfszy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3anrzrwae.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3hjwguybo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3lfarapul.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3umsakbjd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ouyzejdn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ymhroteq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nvnjyxks.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hzltkcrl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mimeakio.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ckmcjkqi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pntauzha.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3usmbgare.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3stggmrxx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vtikfxlq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3chtzhmas.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ekbdelhs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xcwqbnjf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wjcbovcp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3bmugtkix.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3apjftqls.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3rqsxoaaz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vfyyfiae.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gubjdnpo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxuczbvv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cbnntxxv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mtbxrsym.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3inaykwak.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3necfaohq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wdwvleay.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bysqnctn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qsoljuxs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3uoehrtuv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zussodji.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hprxlsre.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3slxeoppa.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zkhmfzwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqsnnprn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3adqcwfmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdcjewkk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3uxxveycd.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gbruroii.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qohpzkfn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3temupdvi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hyzpjxpn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tfzitokh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jactfbgm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3brlgqiqq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kqamlrct.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3iyrpncyv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tcsyjnaj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hiruwzwy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3haeuupkx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tshjsvwx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rctkewbv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3unjhvxqb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wrbnhhpn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3uqabffht.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3moplvdxc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zbiscxyf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qjrmftdx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xxfukfbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wlzpnipx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vsjmpyye.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3glmztsel.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cflqeoug.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sjimhltm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qxwxouse.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qbwoqkdt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gweayemg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ohtityzw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktvopfcn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3puqwyjln.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3onxullvt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lvatxdpz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ssfvjnzc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3omonchlr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tufwiyhj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zrjxawhy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fqidfrgt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xwpqqfzq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lhbqfqvt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tzeinpkj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3usjvbjwf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3febxqpfv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3kcjwukdv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tywykjke.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yqlxmbhe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hxtemceu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3peamdeoc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3oteyfrpe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3qrehytcm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vwlmsspa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjoevdpa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3stoviren.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mftbeyun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxfdpvls.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yxrjniea.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qcqcgmci.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dxqiyebw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3iryqzezd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bqwqhmid.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ylqwrilc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gktydxyc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3tklcechx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qtggoxfy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3rsljjvzr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3iymfpxbc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3prlafrob.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3pykaxhra.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wcgecgri.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3abhfdzyv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3zfylijyv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pkheblel.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3nwtsrfly.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bbzrbgbf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lacbwsfn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbhoncbx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3vomuvmlb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybszrmaz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3frntplrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hotjjwgj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vglekjxq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kenkpugj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhguxiom.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmgvskwv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vtnsaqdt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hwqaagpz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zdzxigzb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xyjozjuy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cbtexpyg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lpkegqcv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxvkvjfo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xaeijwkj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ikzshynv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vabtgdkh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3eqnjzynh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zrhsuloa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mmhaecbx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hvcamgbu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dampjzwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhbtrwyn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3yizvjile.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aruqjqrn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3wnvmyiwt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xpjjnssv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3sllcjdxo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mmsxhimf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yyjexqzj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gkojzhha.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbntyje.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kwabwnsw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3memafveg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fnargmsx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mtqirnaq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nbkyszlm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dvslfdbw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hlfuhlkk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bpktnzzq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3jhkitrnj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3cwrogcyl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cgdibwuc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jbfvrwzh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3fuvqhwbe.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cwuyrvia.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bmejhtey.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nixvbxbv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dijfhbew.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pllxdobk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kshzgpjr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3phiqiptx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3givxcywf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3mfuwifgy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vqonxvgt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xhgkeflg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pvpmeapu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ooikrsls.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kreyxlau.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdkxbnd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tdizxwdl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3exohewvh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wbdvaltc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hmzkryfp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gcwcfamw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wpriaxvm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3spwpowgg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ysndmqco.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nwbhjfff.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oykorvna.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eovkcdca.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sutkmrwj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hndppfjq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gqzfwhts.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wnowdtrj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzyebjq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqbpjmf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xjfbwmkb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmbdahw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3zyjkffxm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtjgoez.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3imrspngy.html


<!-- 参考信息 -->