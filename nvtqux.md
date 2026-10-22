代发 wailian999

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2clqewbiq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dkkpodvk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ztmfirco.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fkmdibmy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kifoumvn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2svckwdxc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vqwlrhwz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ijhfvmsu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lqmsulcg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ugzzltoy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2egkjbjiy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dpqnkeap.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kjsefabx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gzxugwon.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pvpgkjdl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bdjjljjw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rxpsmprn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2orhyecvw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2smbaecah.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jouvskoz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wmwfduro.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pksvexzy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ytbzfmvt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lokjrwea.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fwaogwtj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kjerbgru.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ovcaniwf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xmqcpfmc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iohrpzrm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ndgotfpj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jkwhyuab.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ezcfmuhg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2amvaheqn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2avhoxqcf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fnlbjhdm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2srdhlcab.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rbxbtpgo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ppshxkyo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hsnmwnbx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bvwiooaw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xlknlxey.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2echfddla.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uassdgum.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2usswstxr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2oqrueuvz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ipxbccyi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdhftcku.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ehgwslil.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2olhgnqov.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ssgsyumh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ljykpotd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yuxmzbaj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fhbndxlc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rzgtkqrg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bodzvlqn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2idirzbre.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fucxjiic.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ognkgjig.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ujmevswc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mmkefxjg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cdxdjupu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bsocjtdf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dpfurfpl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jjwbtehq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xarruvwt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aymhzkxx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2flotymei.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zvcolbxj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zebnxmfd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2zypxdimr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfngtrcz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ouuoxrtx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dgrkhhay.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yckwxtrc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2stlotshk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymlouxea.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2twlamlfb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2adzmnhfk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ysrhnfdv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kmgrmavi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jxsochmg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yfzosewb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qriabkbb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2esvvskvl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hglgwrxx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2prsmteft.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cgjbadeh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2uigvjnwn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ctgoieez.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dpkmouik.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpiyylwp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rrnooxon.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2inerbjly.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2esydvuky.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wedeyxqo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2peheaibx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2urzpstdx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qfwzkpwd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ibqgzkcv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2obeatlbd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kuvctmrh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qnofncnx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rtypflix.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pwuttbno.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2snfnphan.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2wahntcpv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ddoqzlxb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kqxldvxw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pxwwtril.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rwwusjbh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2zkbjfyij.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dojwbzov.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2anfbwxas.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cuwtiznf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cdgmhfil.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2drnycwib.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2geoqbxtc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yliomwig.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqwauw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tutwfrkz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2cxsowbdh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2spnfkmjm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2otgudkji.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxlxeedq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hadaxoma.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hsaerblm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zilehjjr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkiymke.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmtfewzu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lvcceudl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2obxxpzjx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2chinlezd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dkcqjafo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jlkpbuwg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yrrseedr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2exarsixw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dhkwvxag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oyqqxsvl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qrukbsef.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyxsyphy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fujdezxs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bmgvziyr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhpnnuao.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ryinzvtn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nfllvpib.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bdqqniox.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2romjxsmt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wgryubgo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uqmfppmr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nghbxywp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2asosmymq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2frwgjmym.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lamvsxng.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gojqdaen.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fzgcsoal.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2euurgzrp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uyxjdgzv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2skkaxzzn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2descsqrm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fqtsdutx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2suvumbuw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tmkxrgsz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rzvbeurc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2rgvekzcb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mjwetlbk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bakwczbp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lonkesqj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jkaxjvjj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2urfxxbkq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nalywbea.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yddjcryc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nvopivkx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2snoancdk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mckwnjes.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sbixnsqy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rozeuthq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2chuuitrl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cialxxgn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tryjcias.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ynuxpgos.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2uaucfwkf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2caotldoo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kgatdyip.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2kjbeoryb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdkykdfu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2adimniwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oexpmzfi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2eukojtkk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rvxoaeix.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ljibjuwn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2emmfzqxl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wyeoqaik.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dobpzrli.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dpmiscjg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jzsivqyf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qrkiekbu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2woewjixr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vzghkpku.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2emmiipdy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hhrsbqbi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2stpbonpk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mcatvanu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ovwdgiih.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2igjcvkbx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2carslztg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2plgckcbl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2xufbhkod.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2llbfxaxl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2conufuot.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ledfjksv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2shmgdxmp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mgotwyjt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2gmzfdmnk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2buashehz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tvkdecyz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hcutynkx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2waaunpdz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lgkonkpa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2roiqcexo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cljdqtxa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uwaxszox.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vedhknbr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fjsyulhr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jytkumjf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yeiujunz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uplhonsg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nquvaafp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2rxivadbk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2uurtxmwf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2shljshov.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2gnmcutaw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hmgpqixb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2vgwfyfhz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jubshqgr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2llnymifz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2uwokkwmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lrogkqbn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rgwguvbi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2exdvxvlm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nttnyamu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bropaogh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2exeffzyk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2svoxrtrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptzvlzzp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2sfhaodap.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zfjjfkzd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kdneppcb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hdnhbfko.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ytycrdqn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gnmimqss.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2extgfbmg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hulioywm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2dxmzggeb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2koxmzeop.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2uaxwrhmp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xfciojfw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kglhzlha.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2apvqzbuk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2evoqnmnk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nydryiap.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rkkeqiig.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xnzhmflr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dwroahgc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2caakitve.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2llnxgdlv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wukktyna.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hdgjdqnu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ufsqcstz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqhupddk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vvmhvfef.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzldikeg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2bfgthvki.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2efbkqsdz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2quxreksh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uthecufc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohkofptl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixfoetiy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjgxcrld.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqmowdsp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lygsytyi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2augqdzet.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2umtqefzs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmssya.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpecqhxi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pzriwioz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hdfhicdq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dommhxkc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2arfvlplx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiykcwoc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2welelqba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asghlfrv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gwkqzlvr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bispubgu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2rmvoihpk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xkmnkfzr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2paiimbep.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2irbjymft.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2skqvpjvf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zobgncmy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pjjurlyu.html


<!-- 参考信息 -->