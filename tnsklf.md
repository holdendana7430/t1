代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gwfmxbsx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ngydkfmz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3phhsgwaw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrmzqat.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cwtnvptv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3owqflcrh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cznrdzva.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3csvcmutc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tcbdiosi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3rfhesyqc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckhrzdvk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wgdewnxm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnixzvke.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3slaqsvcc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwvizndd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3aguxnqkf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zwuqsxxv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tyxdlmbf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3poukjrxq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aabnvtfw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3edyqfdtq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dnenhlvr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pcwwudrf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjtlzupi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dxhrmosv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cnxkxmpo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjyyggfy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dfajimqa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pwbunfoq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ytjmfkxh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fsqatzxf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hdlhawad.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ttzjslvz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fckqjtzj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zcpibsiv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exmsbidy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jjrpmvhf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bvuodwaa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zxfuedeu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajozsmty.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3gptdqova.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yibuyrfw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ubbxuxau.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3scwcuhnn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3nggjoqeo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpfvtkuv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3edxajpup.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yvfymxaq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wkvtuljv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vcmqiido.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rckfbady.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pjdvolnm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mdbziimq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pqyibvfr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3abwgdwba.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vtxxdlll.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xxgtrkka.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cvsktanc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vtwgfgeu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3gsuxzkzw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pcntpooo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3nsizwbxd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmdsyspp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sqqkrxio.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ezwvtypx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pbharhcn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vuqkotjn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nnqkpoos.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lfttrxqe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jnptzwte.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vknaoenv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nceoefba.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jsmetmjs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lmdtjjtf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ezcatmxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jmxqjyoh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xletxvor.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pbulprsc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wahsqaof.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bwwlulwz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mwrqlfju.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wjfgocym.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wuwtsysg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3afrykwva.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3coiptfna.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bmjlatcd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cgrvxkbb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdwquwlo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ifmjmgpx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ohvtkrcc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fptvfwoe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lbawytih.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kconldok.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xjbbjilk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tzyuijbo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fwdcjfkf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gyytgmpf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qsyzizms.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wwalxskp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yecdxext.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3aimkcfuu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tjubjtnr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qasgxznx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zykysspq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eyrmgtly.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mmehnost.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gtbklfye.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybvuudix.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ntviudtt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dzyutrje.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mbsuumfj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ocwxsxgx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tuaebidk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gcatmiqq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ucbknuxh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeqqujsi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nvyxozhv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mgwrsigc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hgzgfrod.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jrexzghh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jaynlwvl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dvoksbhp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3swqsehbv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dhubrvde.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ktftppqs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ymemmtaj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nnpxsurm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kpehsgeh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lgacltly.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jhebvvhv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zifseaew.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ujutamwh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fxbxexcl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3diptfsfd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ggtiozxl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wzavtiqn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3calfclnl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lbwchfxd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mbgitdjc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3feuhsfsx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mdgyjqhx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3audfcjmq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yedwfwrs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3uwlgizub.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qtdhzzso.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jfbxrjkz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qyzazpyk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ubvtrirz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zrzdfeym.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vmdahmwu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tjeqnijk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3efiwhfxh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjdoqj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3peturctc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ecmmelcd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guxxyzxb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vhpnlnud.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vhswnsua.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pwzndeej.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kbxcappp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pybsghmz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uqcfughn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3pobkciul.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3avpdmmmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdgxacze.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3skwranxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvosoyuf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3tabidzbw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3uhruyowa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3iuqzzbnn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ptjmpvva.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zjnqcdfy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xbgzkiwd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eivqojmm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zznwzahd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3potqcnjx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gpsmtoux.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qxmtclkq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zhclljye.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tnxyrbdg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fcckeaho.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yjqfysmp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qtnioqrv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bhsljkcu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hxekaefg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aycchazu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mrunqwvv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xrilnrvu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3exwoukzu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qtzmuvpo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wjirlcit.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yogrmgmg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3demkjdnz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ppwahxir.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3drnwrgrp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3oioquafi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3smqalkid.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pciaseoi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3alcdsipr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tghstjwb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3frxtgfgr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ofmwqets.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3tqjtmzna.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3djzwqxsu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3gayvddvy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tydwlwcp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fnuaxdgl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ulssvmsc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nhqkgbvf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eotavduy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lkfuxika.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pcjglpnk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3flbdenbo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kytfarsv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ywuqgerv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dmdozgxo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3dgsyhgwe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3yvmnsuzx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rndwueuu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3dqxjxygk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsuqjrzc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3vfldiwqh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pyzigoqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbznthsr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ezpcrido.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eghqbwka.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ikgaugng.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bcdbppwx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zqqqqpdy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tssfwvol.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3layobtvl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3plyvwjif.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ngdqoljy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bjirrlrd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3veezsbnu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jbabqxjw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3aezgkmin.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3wcimqdtd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jejwsrqz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vrurbeep.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wmyafycd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3uklcjhpj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3arjuinsa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rarzyvot.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qjeuyigw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3mlhyigwe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3msxxotiy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dyizptpp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3izcmejan.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bkllrvil.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cjabqtzb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eifswxfw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ffjlkopx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kqqpvyha.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nwpmisjy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uablulbv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfqrfvse.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbuwjsbt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3spogjmxi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzklfsep.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3jiflqedy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqbjlrzg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3riffwivy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zhzqopoa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cfpwulhe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3mjjxvnnq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xzxcpggq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwmibnww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhykusgi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xxpikmqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxihzocl.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3rvxukruf.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ktwbpqwf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uurtxrsc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3slhdmlkg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3sfqmppsr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3khbskhao.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rocdzobd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3llnhpgrw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wpprqrhb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3cvlqxhpi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fvvuewpj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cvbusmar.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvgbcimh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3cgyvjqee.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oqdxieau.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3drfmrfcx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xjxmktpy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vnubincv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3gzkftyce.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wgoczhoc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kxabbxkg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3plydquwm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nshduxqm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xjvehccz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rlmkysia.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ucoqcgxu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vjcbfdkc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3abroijov.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cckbowom.html


<!-- 参考信息 -->