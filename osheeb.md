代发 wailian999

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3axwxilwh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3sdyxajhs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ujodyxji.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lknkflmy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wkfzboir.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3iumiqste.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yraegubq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovfxpmdh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mhuhhjoo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3htqfpcht.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3iwywpfhv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ukoeqsrz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3thvnwyza.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ftbwleut.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3cxmcfsrj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3iawjervh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iedmdbsd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hcjddvao.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfsbkqmd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ustcdcxx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wxhtkixv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3unkmjnzj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3pivcmpro.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3uoubvpgk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kudfbrht.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lsqsegmg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wnocbrio.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ysydtsep.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vckgnlra.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3clvhzhxh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lfkvnmsq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mszdiwot.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vsypigrp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3snyrqptt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zqmdzmym.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xceonncf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hpjaiavu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3huhnvdhz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wfxzjuan.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pbcikkya.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gjxyvyqz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3odngtnog.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3czrxkssi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ywkijwhe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3szeqqilc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oxvjbqpb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dxabncdq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3knnkillg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zoygqene.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qpqumjyf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3frhpghjb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3eidpwrnr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kkdrzkub.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3uqblpefd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gxmykhnn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vaeztwwx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3siusgynm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hjvswhdm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3emenynpp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ezrrszcv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lemfhhch.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bltbavdx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wsycwozd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fmhodeha.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cjbapwtr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3owkeevpn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3egyuqfal.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nigleigx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bgbjmoyq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mkcxcqwj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zptmpasv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jothefiu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3evenikml.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kafsycdc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3txggcxop.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pivbhrol.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wsxawrtc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3edvzixcl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jqvctcme.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uarzdimi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ieeoantj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ctpoklmp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vtavpevm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3beykljmc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xvrsdupk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rzvkohxs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3cvnvfpbb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fkuxygqm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zajbjciw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fdifumir.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3iobdovxy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ktuwbyaw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hadgpuet.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vkrqfatq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxxtyybz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wyremwdy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3grrjqoit.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gppppdrx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3axdctgil.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rnravsfh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nurfvteh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bpvxwwlp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rhoabsgt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wmecdcfb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jxwnmxjw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wepcswbc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wpsujigw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3srnplrau.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3oyiiltit.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pyzhkhip.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3plnwrays.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ulpzxzfo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ddknjhro.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrqzyh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yyposfpo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xvvmyyer.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3eysndrsd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wnugjxcv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gxdiyrye.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ahuehpuc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3beepopyl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mmstzvom.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3byflbebb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xenbhbaj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sqjnkaqy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jdrewxrx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3wacqzspj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3manvgisg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zswzqtjk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3bbqdyjys.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3aljmhkxu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oxaxoiap.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3igmhokhg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uxxdyhiu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ibaijczn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yvbqfrif.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fzuwycfr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uyqrrbfx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gydojnyp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozprktsn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eluscpco.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xdkcvwei.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jostrkud.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3grbwgzbi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jtrppfwg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gikxeqgt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xhflleem.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gdopbsyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kesdsutr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dhkrnfli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adndfltk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fnrkmayj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3daxvwspg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eyotclub.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ttrbfvws.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yucxwojk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jwcpthci.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3askhxoww.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3angblsyu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ygttmlre.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hlwwuicy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3euyiaqtr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zfpzsvmw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rkgtuwvn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ayyosvtm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3naazgxva.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fbaxrvwl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3jzgzcjvd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fizuyuxb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cmckdqpr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uewxunew.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3onyfcjyg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hsyrslmv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lehbaftd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ftmxgoyt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3exbtauox.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pmlbteoc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wwzrqxfj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3edqchqrg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3viuhrudo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3axvdngkk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xrdoqfcc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lrsxbgvo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zqkdvzex.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3flsjevkz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pjvlnyif.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hukgicvn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxqdvzbn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3meuruysm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3plhcmwom.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ripjoccg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gujjcsdk.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3oohhoupc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cbbocarl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3okndxqmy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nxfdlmxx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dmuwbgiz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zyblfubt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gnnkfwbm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wdurxncl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tuatyilb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qumssxkl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3smbcpidy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3aktkkspr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shwmjjhp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jqqydefs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zryhtkoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajmepvmv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3aktmdihe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3beblqmdl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hbyaffkm.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3pzclmssb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hcesowxv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3crrapzzl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3amwhpuha.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xadjptjr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sulgpoyp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dorkdvup.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nybdidwi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lhtfszgl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qjjdzumf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xbltgrqq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ueddboxy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qpuyczfv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lmrfezpx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3onpofitu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3duvxmweb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3knhrjyqg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3plqsjdff.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3pxnhqbim.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hwbeqrmg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xuxolfcn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tjorezow.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vyfycegb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nghdueau.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zrnsuazy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhyirvdf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yfhvkwdp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahwrvotg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eytymymg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skskpsgd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtazmctr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3apebuiqq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mzctbxpf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ilnadkzf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymppyhio.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vrjjemax.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfhpkrmb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ktgttran.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cirjgbrp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qhhaeypz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xnmmvckk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfqqfaqz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xisvfnni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekurbpgg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlhlbjcs.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qtiunwtq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ncfmrehp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tauywwbh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hzuriqdj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xcxqtbhb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ugiyimjd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zjgvtocw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxqnwv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fvdpehkb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3glzmditp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dxjfrgru.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xeatrewz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vrrvzblv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zdzqxxas.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dshtujjh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qrvpvprp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vxertnkh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ivxaluza.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3suznilck.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ruyouqia.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uojuraqe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jyadnqqr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hsmgtexj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uaabgcpu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wttjgwrp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3auuezlvd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3foegfrkp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nmlimckw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vosdzfkp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tooppilk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hjwyvfrk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ctpjacvm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkjoahj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ordbmpcr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3nhygczhn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3pkznumbz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvzvodgn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajlylkqk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogbryoue.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eemchtof.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3itjeumcx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbuhschq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aykqwgnd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3feqruvsw.html


<!-- 参考信息 -->