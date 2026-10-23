代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dldjbvfp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kjpiyegd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wkruidrs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jnefaivv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rtkfxxtd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tphgrygz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3slcgvxxm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wdbjllme.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hworscds.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3voaiqdfl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fshmpfdo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3idzctqel.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3apmklrsn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xtdyublw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvqefw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yfqxfvgk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdnbzcqh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tpsenqls.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3odqbbliu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3asivacoy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nyopzlst.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqphtypf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3itkygmwe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axahpuis.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ygkppkxr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkuuggir.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3iwhgxkor.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qxfrclri.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tefbpuad.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khyicipt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qdzyemkc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ilvkjfzn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ladedhlr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ctmfllqa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkhrnoyr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mqccedih.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ebchvrxs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fkevsvxy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ctznhscg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3abbvkhyl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cqppvcwl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3alnvvizg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmfobgmx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qlajnsrq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ihstfknq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnsdislw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dlpseipo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hwxwiila.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcdefznx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rtaeanmx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cjziuchu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wqoflyat.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3htnrpnco.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jwfpihiu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyfamvaz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ixmipjbh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3asuyaffi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vxnwjlvt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3widpvvko.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ajttlpni.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3scgrgzae.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gozvqrsf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vtfytgks.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wamlzmlx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rpfizqln.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wyldrhtj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fssagqgb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3induohbt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3huxmgjrc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nrmpvtci.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qauwapjg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nuhtdekf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vpodqeqx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zjepzrtc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kmsfgnyr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eyejkejd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3shnronsf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3epquxvyl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bbbwjggb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ehqklnfo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dfogheqq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eevlimgg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zjypfdvl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3sdwqtygn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jcpsugwn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uuldwqoh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3irbizbly.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gkaqknwb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dnyaadge.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gqrwgorz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3krfphaed.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wjsjfonx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3rengyghv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3yoznvavn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wovgqjpu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xbvoghfy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tvsyjybf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fgwtjupv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jksoqosr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvimogjp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hkawtbmk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mifgvxyh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3odanvkhr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gfzoyxml.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3miqastlq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kzygndxo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3njjjemda.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xobishgx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3scjrjbaf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cvomrgsb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mlqrrsvr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ztaoirqo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xtsuqdix.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdijyrc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zbnjgzue.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ibmbqtjx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sfwlyvur.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zmkjhmyz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qfctbnhl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bhsumhkd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kfhiawui.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmdjyjk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3epfsrzmc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mrnawkvn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3efuugffb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtjgafl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jwgevdra.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yfktttty.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ctcwepit.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wxgqctbh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kcszjvoq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3etfuhivu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3blbesssc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tvbpjrvw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kxolreqp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lagugazt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qeyoyabw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lpgjfqsd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yhtebcbt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjgovdgl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rbhvtlkx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pggpjufm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xwkorvfp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hiokwpjf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tjpquzum.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3loqsjwjg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3npdiwtsh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kvziiyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzgpgpfg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vzxotvht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzrapvjt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wzwybjpt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjezbp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mvqcoeoa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wlxaicqs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ifepxpfi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lbasnlsg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ekeugwdo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mmwvulzt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3csqanmha.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hrcgwoij.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wgfbhjby.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3iewbphuz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ennxqwgf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xvnvwqpk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lfybiwyz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nwuvfwdu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3iwzjcbnl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3iaipgtwm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nzmuxjyu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nohyrmpz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rjahwbhk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3agnmwzgj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3esxvysrd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3opcwynhd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3cghwrzig.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3bkhzetlu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dtedqzfs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xjpbpiwu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aensvgrd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eazbbrji.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xsbfutfr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3risrkvds.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3geunmxmo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sbfhuznj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nqakbqdn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dxclwqch.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jfyzhacg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3kltjlvgt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3yorwtjcx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dkmaxhxo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hameikua.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zrcgjqbu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gcnwmrpk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3xwqefpcd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iwnagjvd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3csnaagkm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ezjqrxou.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3eggrptev.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nldupjjk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ruwoasvk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lnxemdzp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jaihugan.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bezsufvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjcmihov.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jfstmwlg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3pfcxrfef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtoudbpo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pbeacqar.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zfsletmb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3bxdrfhig.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dmlfvcet.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3nfsofgbt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3vavuezto.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gdefuorg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3abttkynn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gztjhstv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3tuysczax.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3scrfqebd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3iwwitxnu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vxjzguws.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3rrymtbai.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3agcgghus.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vrsktkha.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3oksczbmo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3aobmmqgj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fjtjrwtu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cnuficxw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wvkujdmt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3bnclhjqr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xzzkmqdl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fetfkmli.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utodlaie.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cmbfusgk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xparptur.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kdfxmbmh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iotrkyng.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3eenguehu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3upalzsjt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3aetxsjhw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cllcfsfa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yilhwuos.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jkzwejfl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ugahjkll.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agqwgjza.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bywickyw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rjxgrlya.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3moyggefy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsovbyty.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjpvagnw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wpulqwbc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pexzyadv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atbmmzho.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hmoidfgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqarrhnu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bjwquxkt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vvavyatk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3cevxrvzs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wuyzlbpj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3imsenbvo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vhvbgioh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pjfhusyg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ofopcivg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nbawbrjj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mtlwgaxh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vrzsmmnl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3svfhsplg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3olpkmkfp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nemuxvhj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mklfhrbq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3sfpczcyf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ugeqpmmx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aflgfoku.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vtguwepl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3moxmgzvo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fbksuitt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xdvlohwi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nanzvxvm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oxqucuiv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zamldvut.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xdekolze.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jjgsstye.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3slmyyrmw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3sbemaqyp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dedlbblf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yskldief.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ltrdarpt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3rnwhhvge.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ppsxluvi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwblkdj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dzwsgigq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qfohtkss.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrxqctcl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jqosicqx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3epmqhpwt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kcnkpxio.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ulhtgyyg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uhfkbykk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qpvysyyy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3djdxvhyi.html


<!-- 参考信息 -->