代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cujyokfd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iaqdxsuz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wnuztdtc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3khqvfmxw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aztzzvub.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ewnljsgv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iwbqeppy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qkrtazgp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dkpxstdx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rligkiyz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wzjldyox.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvijikv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3rrqtmnld.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xmbwgpmt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3spynoguy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lfdtwbym.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nlkaemuf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fvbxxgwm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gbakvkng.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fsbsbwos.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xbtncqbg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yujoscql.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lsmpfsss.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mslmatlq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3llrijlai.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yupwtbts.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pquzleea.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ljscelrf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jennjdve.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3okgnumgf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3yjnpvctp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gkgjxjzj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dekgghgq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bxrdprhn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3egjxupkp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3oscrxyzb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ntxbmqeu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rmevkomo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfnmubvo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lfkadlmk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3iomgsvtj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ibagdbhw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rhsgicpj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3daqjogex.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3abumhtyp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ucgnycgz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wumuyouu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3edsztnwk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3gomlpcht.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zkqfkckl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zgzxappm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dnuaxbmc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3uajjxqkk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ztoclqfu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xqecmaqv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dsmrdica.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zmwetqfx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cehdjmnc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3iwylefat.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3muyurbii.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3icscykic.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vplkidhc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qimdbiiv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3bmydlepw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3culliyju.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3svseajpq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmqeva.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dfkxjwsu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vwjaaywn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fandlwhn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3clotvpll.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3brigdcff.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xtzrzwna.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fmzdvjmw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wbgtdslv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vmflypxv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cfwmwsyy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bvtotlpg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3usckjryx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fsfdodrp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3krziyewp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fietiecf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hlpzgwoj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gufiwuhk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nywiyuzb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uujmusva.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3utvkcnfi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3biquagdp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3sxfygmuw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3nmjyjzge.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hmbunnis.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nqwjsomo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qoldywok.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3gdurteim.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lmwsnekr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ncboenzz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zwsbayrz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nuqngskz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xavjaoyr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ddskhzqy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mtfrogvp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3oeqobxrf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ujyyglbh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tfsmjlkg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zcxjttzy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wmfvweoe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bzkbacxf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jfiinoen.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ichnomtv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kvupzxbs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rsldwzks.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3uedlfwud.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmxoku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gnhfjfvk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tuvhgfxg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbnrhzup.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wcwkezfa.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3usckriwl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdgsjfyd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bamoersn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xfxatpkl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3soaclthr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tbyuxggr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qklhoojf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dxrphsac.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dvdccqov.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3juawecuf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3enpggsyv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3buululja.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hkomdhac.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3vtvsgrci.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bhuvqvex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahzcwukk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjktmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgtsujds.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3amekrzvy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jcumyecu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gqfngbjo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ssryrcyt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zdzkhndf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3cihscqvf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bbtwtadg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dtxtaafu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qoofvdfu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3trioojxp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wgxismde.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tfotcvar.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pgejypnv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qrrnjlsp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dovvdzdn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zjyzitqe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cxzjlolp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3psujusvn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uaziaamx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ooxeldbf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vdsxygpu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jtmrvhuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qzljxlci.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pwptkvdk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lssbklud.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3owuezrik.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wsssvell.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gxqtnasi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qipktadv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3patgldyq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tcpacvky.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3drooqcdr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lxyxzmwl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ncfzjtrh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mxsaaeic.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nzbgewmn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dtqlgofh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3guhblqly.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wpzjpehz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nngnbtsi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3exjzvegp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3iozrfsyf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3echrgfri.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xllgknpd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3idsyiaee.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3orvpdydq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jmkiccvl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3idndbulr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3fabrgsuw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3haxrnfbm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3cvtwfjsd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3gerrgnag.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3rfromxjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvwqnxye.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bdckfnzz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qoddjlbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cafgcsmd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3cgoveytc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dnxirglg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lehstppa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3uqjgrmmr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hqxvimhp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xlosdsnj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3kjrgonjf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dgjegtnb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3genstigc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ehryslos.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3nbfvpjis.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3zmmqvatp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3cxoabixf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gzhwlrrf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3cckugnlt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nvhtoefb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nqmpcsza.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3thrdxlap.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3opyimshg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vensboln.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zkarczeu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3nxuorcav.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ybijvthk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eaomemaw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3psgtnphy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vdlclmph.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yccepmzs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdvjuuks.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ldciulyf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zjjscmfw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjsgiix.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3psmgbylr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xhxcuuat.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3izjrwpga.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fcrbptek.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bmxgfgqv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jdoseipt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iuvdcmnv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qiodmsww.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myjqvcxt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uwdvqfzn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ortuxqbs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fkcuvzye.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tbusqjkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcppyhfw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwsjwbqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glrxjdtm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbryzmln.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qbfhrehb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zvemajty.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hdypprku.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ogatkqpe.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tvxrndbx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zhpczatb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3efskhhhj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zkggdbkx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wmblpfep.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zqnphrso.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dcwqcdsx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xibyjuij.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ulztdyei.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fvjfwyxh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dblplnis.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nwkjefqh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yngzmnas.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3trljvghs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jkxliocf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dwzwwpvv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3exlmsrgz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fhuwmcug.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkjidec.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cydqtpgx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rjrkxhkb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qbyetsdh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3acaqcexd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3knootkjr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjoroan.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hpndooad.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lmvyrmgw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ldaypson.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3hdobrxre.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3daaluiwm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3bsudvldb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3didvlsed.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3zwjgmxim.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3niodguxp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3omygfhcm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbhdjnjk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eubgdvkx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdjoswsk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nfzckuuc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hlrmlerh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xdlepoyh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lamkqevz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ynnjarsi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wnwgosmp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xmgrdpix.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nbdtxbyp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3cddgxygs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fawsyoot.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3apqsudav.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3hhekseyf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3umqqbbdm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3csrnyghn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fugrkwfj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ttpiomyv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqawdzhn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3acpuppay.html


<!-- 参考信息 -->