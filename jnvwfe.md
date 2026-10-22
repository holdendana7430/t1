代发 wailian999

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jhvtuffb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zocouvro.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nnyoiiqp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2losmuatt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kweluale.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jeifhtjq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2waxgckzw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2enqqglti.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gvdbzdgm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uxkngkmd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jepzyply.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2yubcwbkb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kvosrnco.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2myqroikx.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fmrxtgzf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fqxvhefs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2alcxsaqn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jecbardc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2naboqvds.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lulqcxaz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uknpqjep.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hoeeifjl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hqgoqtpa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsswkmv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcwmwzzp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ryvsbyuz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2figtnrib.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bolljdtr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2riwddzyw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2uwlquvhq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbqowynu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2egbupjoo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dmecxgia.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zdllwaps.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wttotper.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2woqegubm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rzervfhu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ayjynoaz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yiubcokr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbadrxix.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vdpvgfeh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmicbpyz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2cffvwhai.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqunfuxr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2tuguejah.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmdtxxk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2pryxqoxd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qloquttf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lyrxqkhs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qlcsoqfu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2mmqiksni.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2fhijlsal.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2azgsbmfj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jtxhtplg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spjimmim.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2luycmhib.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xpgpupvh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2enbkrbqw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tnhpsits.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zfaimzhs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fsyljotu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dkryonhn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rbwtfjgn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ovrkjack.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gkmjsgmu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzghrvnr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kidsyzym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qgcwemzn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2soohgpma.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uwexlgkx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kyjmvlpk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hkehjlkb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lpujprxd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2romewtam.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pthppudo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2sikqlvbs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2odkmrltq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rruqtumb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dmqkaspx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2njjgyjzz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qbrvokxz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jwsiglcb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gjibhazb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vbjzremj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fihfyoaq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2csjxmaka.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2gbvhazec.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2uslsttun.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bfngwrdy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2pebzypin.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2prnqevou.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eoqmnxxo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mfantcxu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fabjfybl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zglfsckf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uhhiolll.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2atrkikdn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qgbtwmim.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xaipsvbg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xvaagkwg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hclddgqi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2okpyjdsv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mkwfwdxp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ptzakfpb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lvyyiizz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ctlwaake.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ykhjyswi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxytbd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ewsftpjt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mpbhvdgo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xcaqsfsk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udrbixtf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dipzgacn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oxgypvrn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2olepbqdk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2faguxzqn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kfbsnvjm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2axipddsa.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jyeeloin.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sljdbqqp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ulnplvta.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mrytbpxv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hsnoywtx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qznxglgq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2puyggcxm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2voehzbzd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dnxpwbeu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ntikcdpr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dllzclue.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qybumvqx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ongwvptu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qqztrscm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zvpxlzur.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hgvwqsxc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2guunwmjw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tmmobude.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yszwytgw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hairobun.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gwwydbjb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2iykfvodt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xhvazmqw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sglxlpxx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vpvkynyb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2acfztcle.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2shkrftlx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2arvnwhay.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ehpghnbp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2kzkaxzus.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lczylqmw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xuqjivql.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xgkdwkqc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ozgaspqz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2dmwarixs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hbmlcdez.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rxbrlesn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dutdebwt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jlqxgzlg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ppugqbet.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jkqszhkc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2soquyxcw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rynnawst.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gehnouhc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vznaskcc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xvgllosl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tjrnjtwx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vdvwarjd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2acppjjcn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zzvemlkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynomriwa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2asvuhakh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfplhhol.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zezvcrzx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lgypwclq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vqgpgxio.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jwslyaxw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2iwpalzbe.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jgiqzidz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sqarnaan.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ykiyjyds.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rmjvylyf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nixicxgc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tczkijqt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dbsigtbe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xisuoihp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uitfyuyy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lbudnzej.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2tnhzkwpj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2uxptxarp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yqnwthwi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yehsxyjp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dwcdtzcm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lzgltwos.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2quhdtglf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xvlyaeba.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hmmnxiut.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lbhnsaql.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jdgcvpga.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sqjirdis.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nsqmsycq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jvqwyjor.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ojpbbitn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lxwdvfuw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2asdxxeli.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qhklyzkp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2knkzxynn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jpbbhkba.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jqxvgstr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pqemuuns.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2rqefzimj.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2myaspoja.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kvzrghqs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2eeqebiam.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2irmpczzi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lfxfkzra.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2phmiggyp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jksjlxml.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pniytlhp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2apxuflnt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rfgaalfs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rwczbwdk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pvincpmz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2atkyvtsz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vxbivhcl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2toujdxtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtpeevgg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2itmkkklc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tdmtwglx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnncxeed.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gsjsthun.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rzgidvmc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mwrwghtp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lypdsmet.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2swvjlwmt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hrkcuvkz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xhmletyq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gbwldpks.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2qrgaxvpk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vdrixtle.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vdxsambl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ngokvihw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2avexkwqp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2dehfhptg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ftyuwyer.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ibzxstjw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2eahcjiii.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2fjnqawsi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2byprhfzy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ojkfsvqr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mhfzjqus.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tieghbyi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hubdmrrb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pubepazw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2guphpdwz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dmnzofgr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjpiechb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bjzkguhf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrkihatu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wrzghifs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfthkvkb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrwjmoot.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wdjinuxn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ymkxiafc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lbkizvet.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2seczsyrv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tpgwqzgg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vaefuskx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtiakzaq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2acdbhdba.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdpetcrt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwzrwknt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2zanhvmfe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ylczkqkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qborjuzp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2augktvjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxejvtkf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2txiysfsj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2armclxzi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jaxnyqgy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xojhztvq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2vallothf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tmycupwe.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2boxxsawe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bzklzpzs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2krbuglek.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cdbrghnz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bojakzkz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2actrdayd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2plqjhycw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2iqpcpzft.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wffvtrfp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mbopgips.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qbwxlvvf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zynrroig.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cbaynoak.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lhorqxla.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2szqbkone.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ogfqclbz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sjzbjxxx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xutsscmt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2suaqbzcx.html


<!-- 参考信息 -->