代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.ivvv.top/gtiarrxlra.html

namespace App\Http;
来源：http://hz.hfpthk.cn/gtlarigohg.html

[U44] PHP：开启严格类型
来源：http://hz.hfpthk.cn/gtairbekfn.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtvbimvgom.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sysykeji.top/gtapgadhqx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtsbpxgzvf.html

[U46] PHP：可空类型
来源：http://hz.havefunace.top/gtflneduhi.html

?string $name = null
来源：http://hz.jlsjyb.cn/gtlixwyugc.html

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtkyygaccr.html

int|string $id
来源：http://hz.hnqzz.top/gtjxkkoyzx.html

[U48] PHP：纯枚举
来源：http://hz.yonumen.top/gtnfikwjjp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gteoapixbp.html

[U49] PHP：只读属性
来源：http://hz.daria6918.cn/gtpvihskau.html

public readonly string $name
来源：http://hz.chenzaomai.com/gttyfhqvqb.html

[U50] PHP：构造器属性提升
来源：http://hz.pengpengdd.cyou/gtrbxvvfea.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gthhxklnwz.html

[U51] PHP：数组解构
来源：http://hz.ehwqpu.com/gtobqucuns.html

[$a, $b] = $arr;
来源：http://hz.jinghuilouyu.cn/gtokgmprzd.html

[U52] PHP：箭头函数
来源：http://hz.yangfankeji.com/gtmygsmjjx.html

$double = fn($x) => $x * 2;
来源：http://hz.haohaochexian.top/gtxgftuqqw.html

[U53] PHP：空合并运算符
来源：http://hz.zhengqikj.top/gtmxufxzqt.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gthpmhkhan.html

[U54] PHP：空安全调用
来源：http://hz.hywenlv.cn/gtkzgjlelp.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtxglrjtrg.html

[U55] PHP：match 表达式
来源：http://hz.kuanghao11.cn/gtzesnjlqo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yanxiufei.cn/gtaadymotj.html

[U56] PHP：命名参数
来源：http://hz.aizwys.cn/gtzqkghqlr.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtdurghygy.html

[U57] PHP：字符串插值
来源：http://hz.chenzaomai.com/gtecovscnx.html

"值: {$a}"
来源：http://hz.smart0.xyz/gtdobxwtys.html

[U58] PHP：数组三件套
来源：http://hz.birdmap.top/gtkvyhpfyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gtzyqlocmm.html

[U59] PHP：自定义排序
来源：http://hz.chenlongwang.top/gtmiuuzdem.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gtflynxwmr.html

[U60] PHP：JSON 编解码
来源：http://hz.guowangkeji.top/gtykcjtllz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinghuilouyu.cn/gtaeqqluqt.html

[U61] PHP：正则
来源：http://hz.yuxming.cn/gtcdmlofvv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gthcsreikr.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gttcaabxjx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtwbdeaoud.html

[U63] PHP：文件读写
来源：http://hz.haohaochexian.top/gtllwgygro.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigfzy.top/gtcquyagjh.html

[U64] PHP：目录遍历
来源：http://hz.daria6918.cn/gtkyafojgy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtuprcyscm.html

[U65] PHP：会话
来源：http://hz.xinyue.icu/gtvvhwjpks.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xziqi.cn/gtcqstwkrg.html

[U66] PHP：设置 Cookie
来源：http://hz.jinqigufen.top/gteqihmxwc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtshrfsbwe.html

[U67] PHP：处理文件上传
来源：http://hz.tianlin.xyz/gtevzcvljl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangdashe.top/gtlictdanl.html

[U68] PHP：PDO 连接
来源：http://hz.yonumen.top/gtvlqtzuyl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.316326.xyz/gtzhcxcyid.html

[U69] PHP：PDO 预处理
来源：http://hz.zhongyouzk.top/gtfcmssdck.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ehwqpu.com/gtwwjxchsn.html

[U70] PHP：PDO 事务
来源：http://hz.svipenyu.cn/gtagwjeqhz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jianghu66.top/gtmapsalop.html

[U71] PHP：抛出异常
来源：http://hz.pengpengdd.cyou/gtlpiwysil.html

throw new RuntimeException("失败", 500);
来源：http://hz.zycfv.cn/gtsiimrwdn.html

[U72] PHP：写错误日志
来源：http://hz.zhiwuduotai.top/gtxwkuakbo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hfpthk.cn/gtfzimfvin.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinyuanbaomall.cn/gtrzkhcwic.html

parse_ini_file("config.ini", true)
来源：http://hz.shzxlz.cn/gtcfrxyidc.html

[U74] PHP：读取环境变量
来源：http://hz.jlsjyb.cn/gtlruvhsqq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhijiandao.cn/gtubrliydx.html

[U75] PHP：依赖注入
来源：http://hz.nwbrower.top/gtefxqtjho.html

composer require psr/container
来源：http://hz.zhijiandao.cn/gtalozndiv.html

[U76] PHP：简单路由
来源：http://hz.mhx1999.top/gtqredgnaj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gogol.net.cn/gtkpyrhrxd.html

[U77] PHP：模板渲染
来源：http://hz.jianghu66.top/gtpljovppz.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtrvippdkd.html

[U78] PHP：单元测试
来源：http://hz.dianchejie.cn/gtldudylpr.html

composer require --dev phpunit/phpunit
来源：http://hz.yuxming.cn/gtctzyjcua.html

[U79] PHP：静态分析
来源：http://hz.jqgufenzy.top/gtuvhemnsq.html

composer require --dev phpstan/phpstan
来源：http://hz.yonumen.top/gtmfjxjwiv.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtpbjdlyri.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuetiantiany.cn/gtmxahubzz.html

[U81] JS：初始化项目
来源：http://hz.aibaodan.cn/gttssurtsx.html

npm init -y;  npm i express
来源：http://hz.cashguo.top/gtybrrxhio.html

[U82] JS：package.json 脚本
来源：http://hz.0kj1m.cn/gtkcoaewmf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jyoumei.cn/gttxjykmbw.html

[U83] JS：ES Module 导入导出
来源：http://hz.yj20258888.top/gtuowqxfiz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.sweek.top/gtmbtvxebj.html

[U84] JS：CommonJS 写法
来源：http://hz.zhoulong.xyz/gtuvfymovz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtnmsvbnro.html

[U85] JS：可选链
来源：http://hz.meibo888.top/gtccklajqj.html

a?.b?.c
来源：http://hz.xziqi.cn/gteafnlxgi.html

[U86] JS：空值合并
来源：http://hz.hongshengwenyu.top/gtdlyzzqib.html

a ?? b
来源：http://hz.guowangkeji.top/gtsyioagsb.html

[U87] JS：解构默认值
来源：http://hz.ydjk.org.cn/gtdwnrsvtt.html

const { a = 1, b = 2 } = obj;
来源：http://hz.pengpengdd.cyou/gtzxnzijfm.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gthllfodnd.html

{ ...a, ...b }
来源：http://hz.9152youxi.cn/gtvmhzlhlx.html

[U89] JS：数组去重
来源：http://hz.cqqwz.cn/gtweawtoco.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtbnohkqad.html

[U90] JS：数字数组排序
来源：http://hz.feifeiyinyue.top/gtoijixmhc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtbwzkavri.html

[U91] JS：对象键值遍历
来源：http://hz.cheryme.top/gtjqgigvss.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.meibo888.top/gtrieyuhbt.html

[U92] JS：深拷贝
来源：http://hz.jinghuilouyu.cn/gtyqomttjs.html

structuredClone(obj)
来源：http://hz.cashguo.top/gtwoaflbdo.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtxdodkdtz.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtmscjvuum.html

[U94] JS：箭头函数
来源：http://hz.sufxvd.cn/gtzuexoxpd.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtjmulpghd.html

[U95] JS：Promise 包装
来源：http://hz.tianlin.xyz/gtsjeubwad.html

new Promise((resolve, reject) => {})
来源：http://hz.redwolf501.top/gtyvccepqf.html

[U96] JS：async/await 与异常
来源：http://hz.dashuyun.cn/gttppodqgd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtunntgxaz.html

[U97] JS：并发请求
来源：http://hz.meibo888.top/gtrllkufre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtmiegswhf.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhongyouzk.top/gtnxpblyqi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sufxvd.cn/gtxrjbmgnh.html

[U99] JS：事件监听
来源：http://hz.shangyingyoupin.top/gtvugwcelb.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtivxexwdj.html

[U100] JS：DOM 查询
来源：http://hz.zhengqikj.top/gtsemimyvs.html

document.querySelector(".item")
来源：http://hz.daria6918.cn/gtiebegciy.html

[U101] JS：classList 操作
来源：http://hz.ydjk.org.cn/gtqlsateos.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtccatumct.html

[U102] JS：本地存储
来源：http://hz.zhaomingkeji.xyz/gtxfcbgcth.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuxming.cn/gtwbiokgwf.html

[U103] JS：定时器
来源：http://hz.yongpay.top/gtewjjsomx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhixingplan.top/gtixzxeoau.html

[U104] JS：防抖
来源：http://hz.cqqwz.cn/gtmngqkbel.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtxbcxrqfg.html

[U105] JS：节流
来源：http://hz.bjfxy.top/gtcemmddro.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtcankvtzq.html

[U106] JS：日期格式化
来源：http://hz.snrcjt.cn/gtxnuqmere.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jlsjyb.cn/gtmcxccjqw.html

[U107] JS：数字千分位
来源：http://hz.andypj.xyz/gtbbnklrlx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gtdzzucnng.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gtsozwztlx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtjfvteuqj.html

[U109] JS：数组分组
来源：http://hz.fengsongda.top/gtlutufzxx.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gttfzzghzh.html

[U110] JS：数组分块
来源：http://hz.xziqi.cn/gtqwcacawh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydzc1.top/gtfjkswsib.html

[U111] JS：对象转 Map
来源：http://hz.9152youxi.cn/gtlwthtaem.html

new Map(Object.entries(obj))
来源：http://hz.gaohongyu789.top/gtuawxkipz.html

[U112] JS：字符串补位
来源：http://hz.xinyue.icu/gtaaanlqld.html

"7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtmammzzwe.html

[U113] JS：正则替换全部
来源：http://hz.ehwqpu.com/gthowekdda.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gthpytgltg.html

[U114] JS：JSON 深比较
来源：http://hz.yueranfly.top/gtoybxdend.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.fzhhl.top/gtyautnjry.html

[U115] JS：生成 UUID
来源：http://hz.daria6918.cn/gtpmrnjfbt.html

crypto.randomUUID()
来源：http://hz.yueranfly.top/gtxzfgtoqq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.bjfxy.top/gtdcmocalo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.shuidangran.top/gtxzvmszyy.html

[U117] JS：单元测试
来源：http://hz.pengpengdd.cyou/gtmprhlqvy.html

npm i -D vitest;  npx vitest
来源：http://hz.cqqwz.cn/gtepwszjdj.html

[U118] JS：开发服务器
来源：http://hz.yangfankeji.com/gtupkoeqnr.html

npm i -D vite;  npx vite
来源：http://hz.redwolf501.top/gthuzayfyb.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangkeji.top/gtngfhgtjw.html

npx vite build
来源：http://hz.zdqjudy.top/gtmxzpffoe.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.52xcode.cn/gthgmvtxxf.html

import.meta.env.VITE_API_URL
来源：http://hz.mhx1999.top/gtfzbmjufj.html

================================================================================
来源：http://hz.wangdashe.top/gtyhqgyjfu.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtvgatswmt.html

================================================================================
来源：http://hz.haohaochexian.top/gtqsztrmxn.html

按语言统计（条）：
来源：http://hz.svipenyu.cn/gtufsvfkrr.html

Python ......... 252
来源：http://hz.9152youxi.cn/gtnzsjpzay.html

PHP ............ 252
来源：http://hz.hywenlv.cn/gtikfrdvqt.html

JavaScript ..... 252
来源：http://hz.hfpthk.cn/gtgjxkglra.html

TypeScript ..... 212
来源：http://hz.jyoumei.cn/gtptimrnmg.html

Java ........... 212
来源：http://hz.kuanghao11.cn/gtwomlhftn.html

Go ............. 212
来源：http://hz.sysykeji.top/gtejkvcgvh.html

Ruby ........... 212
来源：http://hz.redwolf501.top/gtqpudcgbr.html

C# ............. 212
来源：http://hz.chenzaomai.com/gtxujlsfst.html

C .............. 30
来源：http://hz.mhx1999.top/gtshbrdmwx.html

C++ ............ 30
来源：http://hz.bjfxy.top/gtlxphgwzn.html

SQL ............ 90
来源：http://hz.jyoumei.cn/gtqbxsszek.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtaygsgwcx.html

Kotlin ......... 15
来源：http://hz.aibaodan.cn/gtonsavupr.html

Swift .......... 15
来源：http://hz.sufxvd.cn/gtnnljeuqm.html

Lua ............ 10
来源：http://hz.xinyue.icu/gtzqqvjrez.html

Perl ........... 10
来源：http://hz.nanxuanxn.top/gtnuiksgzd.html

Scala .......... 10
来源：http://hz.zhoulong.xyz/gtpeilnaet.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtlzmszbrj.html

合计 ........... 2106 条
来源：http://hz.xylfe.cn/gtrwvzvwkh.html

按章节统计：
来源：http://hz.xuanzx.com/gtykgdgkbe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtyvbezjas.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtcdhkcdit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj202588.top/gtfpjilbkm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ydzc1.top/gtxfuivnde.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jqgfzy.top/gtshcivdbr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ywan-chungtsiang.top/gthmjlrimy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ybcxt.top/gttsohfkzj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.smart0.xyz/gtnpsikmou.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtqwreeyah.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jyoumei.cn/gtcamkdbnz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gtrwspswdp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtlsiiubxl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtimhrrhdb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtqcomstrk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinqigufen.top/gtrgbxtieb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gthwqjvoqy.html

Q SQL 专题                              90
来源：http://hz.vqdsnc.cn/gtqlcwpjym.html

R Bash 专题                             80
来源：http://hz.zhongyouzk.top/gtxghsmdlc.html

S C / C++ 专题                          60
来源：http://hz.hywenlv.cn/gtdmookmyk.html

T 其他语言补充                          60
来源：http://hz.smart0.xyz/gtzmflqtej.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtgisvwcno.html

------------------------------------
来源：http://hz.jinqigufen.top/gtiqiyyepr.html

合计                                  2106 条
来源：http://hz.mhx1999.top/gtsrcdiqtl.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtdmcgyqfh.html

使用提醒
来源：http://hz.hfpthk.cn/gtkqxdrnqn.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtwyhpumex.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.316326.xyz/gtioasxaro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hammf.cn/gtajxngyvk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aibaodan.cn/gtarwvpsqz.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxinkj.top/gtzhiscath.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhaomingkeji.xyz/gttbtfyjsw.html

—— 文件结束 ——
来源：http://hz.chenzaomai.com/gtzbhjvpyz.html

================================================================================
来源：http://hz.nanxuanxn.top/gthlfjuwdl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.birdmap.top/gtyccvimdf.html

Common Programming Examples Cheat Book
来源：http://hz.haohaochexian.top/gthbtjcbio.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtutbyxfpv.html

【收录内容】
来源：http://hz.fzhhl.top/gtkxblbjlz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhixingplan.top/gtfaapegny.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cashguo.top/gtovsaupem.html

SQL · Bash · C · C++
来源：http://hz.zhongyouzk.top/gtsfpgchnn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.aizwys.cn/gtwamodgal.html

【使用说明】
来源：http://hz.xingfuxueyuan.xyz/gtdoxxhtrs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuxming.cn/gthhbevnhm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tanke756.top/gtayhgfgzc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gtnbljxxvb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.0kj1m.cn/gtngdwnkrj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ppjwa.cn/gtfrjuostj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtgwbaxwea.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shangyingyoupin.top/gtyxoyucte.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xziqi.cn/gtllobbwrt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xziqi.cn/gthbchiuin.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtftckjmgx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhijiandao.cn/gtyuhphemv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.andypj.xyz/gtwabwmtik.html

【文件统计】
来源：http://hz.9152youxi.cn/gtxqsgqltf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.svipenyu.cn/gtgmiyvjmh.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtpavdlmzl.html

目  录
来源：http://hz.chenlongwang.top/gtektnclwh.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtwmcmhgms.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.fzhhl.top/gtxmqppffb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gtlbatfwka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.haohaochexian.top/gtambvlpgo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtvainjezq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.daria6918.cn/gtfusfjurz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yueranfly.top/gtcwlzoijr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtoubeppum.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pycfn.com/gtkujggkso.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gttffouujc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtbqgvpkcr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtkxghlcok.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gzhubu.top/gtbpuddmwr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtyizgnyqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gtecqjtxiy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sufxvd.cn/gtajuxwuas.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtnmkgxsmo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.guannengcc.top/gtcrloicno.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sufxvd.cn/gtgfediduf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gotoacloud.top/gtzutlwstk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtbbkdeqyg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtimtwokiu.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttpxjwcmv.html

A. 基础语法与类型
来源：http://hz.kuanghao11.cn/gtwslvqaov.html

================================================================================
来源：http://hz.yonumen.top/gtexocjgcv.html

[A01] Hello World
来源：http://hz.52xcode.cn/gtlgwazwfs.html

Py:   print("Hello, World!")
来源：http://hz.zhengqikj.top/gtgwhclknu.html

PHP:  echo "Hello, World!";
来源：http://hz.zhiwuduotai.top/gtckdtadau.html

JS:   console.log("Hello, World!");
来源：http://hz.9152youxi.cn/gtoycnptmd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xziqi.cn/gtiqavstmw.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtrwicctvy.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ybcxt.top/gtckcplhxl.html

Ruby: puts "Hello, World!"
来源：http://hz.guannengcc.top/gtiemqdxge.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hysaishi.cn/gtqunrsoic.html

[A02] 变量声明与赋值
来源：http://hz.kuanghao11.cn/gtzcnwsvga.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinqigfzy.top/gticnmbrer.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.birdmap.top/gtsluabsfc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenjidiqi.icu/gtkcsesupz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.havefunace.top/gtembqjfny.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jianghu66.top/gtlesbujud.html

Go:   name := "Alex"; age := 20
来源：http://hz.tanke756.top/gtbsdhyrqm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hfpthk.cn/gttvnztauq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jianghu66.top/gtfminbytg.html

[A03] 常量定义
来源：http://hz.zdqjudy.top/gtafhghwwr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pycfn.com/gtxktnzxbv.html

PHP:  const PI = 3.14159;
来源：http://hz.bjfxy.top/gteisoudpl.html

JS:   const PI = 3.14159;
来源：http://hz.hammf.cn/gtjvrbretu.html

TS:   const PI: number = 3.14159;
来源：http://hz.chenzaomai.com/gtlgvfucdu.html

Java: static final double PI = 3.14159;
来源：http://hz.guannengcc.top/gtfbiwdymk.html

Go:   const PI = 3.14159
来源：http://hz.vqdsnc.cn/gthqmyhwwb.html

Ruby: PI = 3.14159
来源：http://hz.yanxiufei.cn/gtlizdcahg.html

C#:   const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gttjwbzfvp.html

[A04] 判断变量类型
来源：http://hz.jlsjyb.cn/gtndxzvjwn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.daxiang520.top/gttrzbmphy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gtidvmvzrs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtsahflekt.html

TS:   typeof x; x instanceof Date
来源：http://hz.daxiang520.top/gtkegxnden.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.wangshuangyany.cn/gtoxdiwgrl.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.fengsongda.top/gtbmfhiqwh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.redwolf501.top/gtaibxyrqf.html

C#:   x.GetType().Name; x is int
来源：http://hz.c1oappe.top/gtrymnbeyb.html

[A05] 整数除法与取模
来源：http://hz.xingfuxueyuan.xyz/gtpldspfmn.html


<!-- 参考信息 -->