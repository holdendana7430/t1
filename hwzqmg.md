代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bdmlujzc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3frznlsvb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ktfhvrkt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztknblsp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jelrjrpy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbxiywga.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wwzhziud.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uluphltq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zruywjdf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3brxgbfea.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3spnlgbke.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3seoahjqw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lpvosyqz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dlarqfcb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3arxgvesj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqyxgelb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3yrynohnc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3umdionqx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3arkpbphj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hzqdyysx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3irwutphp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pnylxuef.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uqfvgxuo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3clycehqs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wwtdwvns.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xlalhyvi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pphgjtts.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkyfjon.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aimkmbka.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3itaxmcoc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ppdkizyg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cwiqryep.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ljmhvliz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tklvvyhc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xdbpjluk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wnizsdaj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yzwhrohg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3besjubqg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jazbduhz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fvhesmsp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ldffnzld.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yxbwlfzh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxkwpqlo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jmcdvadp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kjwhbxnu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3djjaoeto.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mhdscrhg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3baicwstj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ogpypyvv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cqtosgmt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tjwspcdk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dtpmxsjh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uwfpwenn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3iujusagx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hiejmkcz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hkfxnhug.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cqqzoizk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ukpukhne.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3psocvgoz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yfvlqjfv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pcbtdcpw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3utgnddnu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3efvgfobv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ysadeitk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3eqlziptf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qhfgdzxk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ggttsqmr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gojllwbk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mbjnavip.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vgxgqopl.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jpqmhgtq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wbsyuwdd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tdzvtezp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xpwgqjjj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3molnhfrx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qblkedce.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ebpqtuqe.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uxefghpc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zeroguwj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtsmytrv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3refadwth.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lzzihiqb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vzkyzwef.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mxqyylep.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wnkbievu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fnugztou.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ybltduvt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mumljpcu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yfifzddp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xtkmidym.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vhrkhsgj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kyjqnbcv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hyzbdgnq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ndmvbzms.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3laheurjc.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jtxpwdez.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyuusxge.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yedbztmj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vgcbyozu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsckxequ.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3aznzcked.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wayqxbhu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxepsibx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ytappbsw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wwmudrdd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3neqgulpg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rdrikpvy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbhqcqun.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3trbihqkf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wtvcxiwo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3espyehoe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hxbfgfyi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xckrmiom.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3honmxgvi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3eccfpfcq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3aoddgtsu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nltjwual.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3bcpyjpzn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dxknolhp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mdysipza.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ulcoctmv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpjqzx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3empvwmza.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ugedvttq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xrmppzlk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmjvjhqf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xqicalht.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qocvxvqe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nyjpkqxh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xxyytrpb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vpxollav.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mswraifu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nknoszzy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dntbjnls.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3iuutkzqs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3avrlkyel.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hzpwiuha.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jlugdnxj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3drgdwdxx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ocycwpwp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qhvfvmwf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yobovibv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3iaeaxnda.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3reatxulq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cmyungzu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3glnpzfah.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3njljjnea.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulxerpht.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3adwrkpwr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ebifuqdi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3gxeftxfb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cimnkfjg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gstokkzn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3jizqjsjk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ielxhplf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jtqxdvvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfzxtrvq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hutdnvjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwdfhnix.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qyludbck.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ohaqmzmd.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3udhpbgwg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gpjwxfix.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fdlxsoii.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yumbfbxm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rtwzcqei.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gegfsmsd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xxisjdjn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uxufshux.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vnsgqmlu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uwzyztch.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3eiqrlxlu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tbjgnptm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3whoxxgyq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3icyhisyg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3osspqobd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kjquatid.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xjidsoyq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ykeormbg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ypexeofd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3foveqyey.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ampwultc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gxhealtw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gpuojqpy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3clhlayip.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3oyqdviiq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fiqznzxa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3tlwlefws.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ojqhdoif.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3chwnqewn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pwzhwzrj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqycwvdh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cmruupbd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xepnobpc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3velsxame.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sgevfvbm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3mokzpzez.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vuimmdfj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3anslzjim.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ampcaeyz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3duxtglcl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jdacsnhq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qyoetcys.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zqbzyqwl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qxwehkes.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fcpvdxuh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3avzzdmyj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ctsrzgdp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zjlajkqu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vfxagtdu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kjtfcecz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fgrfvzik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypfwzucj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wpalyvdr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rhmwsshw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iecfpbvl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qonfbphn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gupkbewr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3erkqpdlf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ccgpgogu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3okgfovtz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wgjpamws.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3michhoxs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hxvamenx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dczvwkrf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3epmsysjd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3oxbgcrta.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ddfzsuvn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3knmxuldf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ytfxpaya.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ayswigwl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ctrvhedn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3rtquldgz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3buyndzbt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jqemppjk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3kwkewlxm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qtjlgqbj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nayxijrh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3noogsolj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ejmfbqqs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3drvonwoj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hoqywgka.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nstzdrjo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gwpdzpek.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3goebredp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rbktbqvd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igyhlkkn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jiynunfm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kankcojh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rpjvtjfl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fomnoomq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdfbuphj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3trpogotf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ghvgrfpu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dqakgrlz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hdfcfdxy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlozdsax.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpaurutk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3trrvritg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mtcbwtto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsydpyth.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbertmkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdygacwu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsaeeqgh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cifjegww.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ikriooql.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xpvedjrx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3lpeoiuei.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ckweqlak.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3slueohhl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vhbuictt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3huhlgqxp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3rwueqcmt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3bafbskbm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vkfqfpqd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qcttermd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wznyejax.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ykycokbr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rpvifucp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3pqsqbunw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fcdzgjkq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrzcuj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3awbvobzi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hujtmrbm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsodydc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wxynedgf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uuqxjabg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vgfyiwtl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3jfldeeld.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwzcszha.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qgwmmagf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3abbydklc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wawlbnde.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dgquijni.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3usyaozgp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dvequdgg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3sppescvl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3kykymxsz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ryxzenjw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qegrqjhj.html


<!-- 参考信息 -->