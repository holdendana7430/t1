代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.yongpay.top/gtrgkecocr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtvnbqctwu.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtkfhbmfwb.html

?string $name = null
来源：http://hz.jlsjyb.cn/gtolunsvig.html

[U47] PHP：联合类型
来源：http://hz.ywan-chungtsiang.top/gthpfzwtsh.html

int|string $id
来源：http://hz.daxiang520.top/gtuibtruhn.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gtvqubdrwl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhijiandao.cn/gtqavnndad.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gtppwpwbsb.html

public readonly string $name
来源：http://hz.zhengqikj.top/gtuykbfdrn.html

[U50] PHP：构造器属性提升
来源：http://hz.zhengqikj.top/gtijumkobw.html

public function __construct(private int $id) {}
来源：http://hz.sweek.top/gtlvyzvznp.html

[U51] PHP：数组解构
来源：http://hz.ppjwa.cn/gtfygudhak.html

[$a, $b] = $arr;
来源：http://hz.gaohongyu789.top/gtcoclabpg.html

[U52] PHP：箭头函数
来源：http://hz.ydjk.org.cn/gttmmwgmnk.html

$double = fn($x) => $x * 2;
来源：http://hz.zhixingplan.top/gthxvexjjl.html

[U53] PHP：空合并运算符
来源：http://hz.jinghuilouyu.cn/gtbrebwbso.html

$v = $a ?? $b ?? "default";
来源：http://hz.jlsjyb.cn/gtvxcjtrhe.html

[U54] PHP：空安全调用
来源：http://hz.zhongyouzk.top/gtlwmmkepa.html

$obj?->method()
来源：http://hz.yanxiufei.cn/gtcsjmyxde.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtryjynykz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yonumen.top/gtmoyfoegs.html

[U56] PHP：命名参数
来源：http://hz.52xcode.cn/gtphmeasvz.html

f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtmivfzrul.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtmtasshlz.html

"值: {$a}"
来源：http://hz.jqgufenzy.top/gtryanjtnx.html

[U58] PHP：数组三件套
来源：http://hz.gzhubu.top/gthwpuyktz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aibaodan.cn/gtdmurreqc.html

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gtkvuqaefe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sxryk.cn/gtmdqtqfmz.html

[U60] PHP：JSON 编解码
来源：http://hz.daria6918.cn/gtvlnlbzgd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hysaishi.cn/gtmbrgubbg.html

[U61] PHP：正则
来源：http://hz.shanyushiyangkeji.top/gtmnswtbvm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtgozsbfpw.html

[U62] PHP：日期对象
来源：http://hz.hywenlv.cn/gtlrrplbbh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.redwolf501.top/gtmqdkixvr.html

[U63] PHP：文件读写
来源：http://hz.jqgfzy.top/gtwcwfbxnr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sysykeji.top/gtokhrmxfe.html

[U64] PHP：目录遍历
来源：http://hz.xziqi.cn/gtjoxddwes.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtyienyugn.html

[U65] PHP：会话
来源：http://hz.jinqigufen.top/gtmywbphya.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guannengcc.top/gtxekoryeg.html

[U66] PHP：设置 Cookie
来源：http://hz.redwolf501.top/gtmjzyabgm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangdashe.top/gtsstdqrmk.html

[U67] PHP：处理文件上传
来源：http://hz.hysaishi.cn/gtvimblgoa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.meibo888.top/gtisiflcao.html

[U68] PHP：PDO 连接
来源：http://hz.yj20258.top/gtwgooifal.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ybcxt.top/gtzqtpoecx.html

[U69] PHP：PDO 预处理
来源：http://hz.dianchejie.cn/gtcqvguzbv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zdqjudy.top/gtvhhxsazv.html

[U70] PHP：PDO 事务
来源：http://hz.gzhubu.top/gtdnpflruk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cucudq.cn/gtooewubed.html

[U71] PHP：抛出异常
来源：http://hz.zdqjudy.top/gtlmkniqya.html

throw new RuntimeException("失败", 500);
来源：http://hz.cucudq.cn/gttennifjc.html

[U72] PHP：写错误日志
来源：http://hz.sweek.top/gtrlpavlyy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydjk.org.cn/gtiwoanoqk.html

[U73] PHP：读取 ini 配置
来源：http://hz.mhx1999.top/gtiyfkbsud.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtvsqztlzl.html

[U74] PHP：读取环境变量
来源：http://hz.nanxinkj.top/gturmjlngz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhiwuduotai.top/gtbqxnyrbk.html

[U75] PHP：依赖注入
来源：http://hz.xziqi.cn/gtiwwaisjo.html

composer require psr/container
来源：http://hz.ivvv.top/gtaxrujnqh.html

[U76] PHP：简单路由
来源：http://hz.yuxming.cn/gttjvtylhv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtwqarandi.html

[U77] PHP：模板渲染
来源：http://hz.quarkkingdee.top/gtbcolitex.html

composer require twig/twig
来源：http://hz.9152youxi.cn/gtzjapumvc.html

[U78] PHP：单元测试
来源：http://hz.gaohongyu789.top/gtxybzlayg.html

composer require --dev phpunit/phpunit
来源：http://hz.shzxlz.cn/gtzjvvlgxp.html

[U79] PHP：静态分析
来源：http://hz.yangfankeji.com/gthhyfflde.html

composer require --dev phpstan/phpstan
来源：http://hz.zhongyouzk.top/gticsmxzuw.html

[U80] PHP：代码规范修复
来源：http://hz.gaohongyu789.top/gtuadpwbrp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.ydjk.org.cn/gtbqoitjhc.html

[U81] JS：初始化项目
来源：http://hz.0kj1m.cn/gtvjgmsdqe.html

npm init -y;  npm i express
来源：http://hz.hammf.cn/gtmgaikodj.html

[U82] JS：package.json 脚本
来源：http://hz.jianghu66.top/gtqlyrutbl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinyuanbaomall.cn/gtgorxfxxf.html

[U83] JS：ES Module 导入导出
来源：http://hz.havefunace.top/gtflolbrpq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hnxiangtu.top/gtrsjejojk.html

[U84] JS：CommonJS 写法
来源：http://hz.sweek.top/gtcgpnyash.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gtaeqlzuxd.html

[U85] JS：可选链
来源：http://hz.ehwqpu.com/gtaerbfhjb.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtagjzkqdq.html

[U86] JS：空值合并
来源：http://hz.aibaodan.cn/gtbdqigjjx.html

a ?? b
来源：http://hz.zycfv.cn/gtvzydyztk.html

[U87] JS：解构默认值
来源：http://hz.nanxuanxn.top/gtfezkrsdo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xziqi.cn/gtqobwnwkn.html

[U88] JS：对象展开合并
来源：http://hz.tianlin.xyz/gtdgeoutmg.html

{ ...a, ...b }
来源：http://hz.ivvv.top/gtbilzrxhx.html

[U89] JS：数组去重
来源：http://hz.jianghu66.top/gtqgzlypyt.html

[...new Set(arr)]
来源：http://hz.guannengcc.top/gtscsioraz.html

[U90] JS：数字数组排序
来源：http://hz.pengpengdd.cyou/gtlumedpub.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtlggzgchl.html

[U91] JS：对象键值遍历
来源：http://hz.fengsongda.top/gtefvkjzsp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tanke756.top/gtewmhmaat.html

[U92] JS：深拷贝
来源：http://hz.chenzaomai.com/gtkdtblrpp.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtmsevsjsu.html

[U93] JS：模板字符串
来源：http://hz.redwolf501.top/gtaolwlduh.html

`共 ${n} 条`
来源：http://hz.c1oappe.top/gtxtbxgfvx.html

[U94] JS：箭头函数
来源：http://hz.jinqigufen.top/gttessespz.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gtodjvocfr.html

[U95] JS：Promise 包装
来源：http://hz.zhijiandao.cn/gtfltrejfj.html

new Promise((resolve, reject) => {})
来源：http://hz.ywan-chungtsiang.top/gtxjeaakey.html

[U96] JS：async/await 与异常
来源：http://hz.jinqigfzy.top/gtrivjmeuj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtcguptbyp.html

[U97] JS：并发请求
来源：http://hz.zhijiandao.cn/gtdjfdgxcv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtoxlynveb.html

[U98] JS：fetch 带 JSON
来源：http://hz.tian-w.cn/gtkmjbmmbj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtqntzujzz.html

[U99] JS：事件监听
来源：http://hz.dashuyun.cn/gtibeunhza.html

el.addEventListener("click", e => {})
来源：http://hz.ybcxt.top/gtupclssnh.html

[U100] JS：DOM 查询
来源：http://hz.haohaochexian.top/gtlumqclsi.html

document.querySelector(".item")
来源：http://hz.sysykeji.top/gtnaxetnix.html

[U101] JS：classList 操作
来源：http://hz.yuxming.cn/gtkacvekmx.html

el.classList.toggle("active")
来源：http://hz.yj202588.top/gtyexdqbpl.html

[U102] JS：本地存储
来源：http://hz.smart0.xyz/gtjjblywwg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hongshengwenyu.top/gtjmsvaxip.html

[U103] JS：定时器
来源：http://hz.cdnleiting.top/gtwzbededl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenzaomai.com/gtpdehmlkk.html

[U104] JS：防抖
来源：http://hz.hnxiangtu.top/gthpeodhfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtrikvskjv.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtpuufrkhc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenjidiqi.icu/gtzlxjqkxy.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtriitzcva.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.kuanghao11.cn/gttlmrqpgb.html

[U107] JS：数字千分位
来源：http://hz.dianchejie.cn/gtawrrbujb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhixingplan.top/gtwlcbzjwh.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gtuwonhbur.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ppjwa.cn/gtzufalsef.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtmvalbpuw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.bjfxy.top/gtqelifixf.html

[U110] JS：数组分块
来源：http://hz.9152youxi.cn/gtlzmrxxea.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.aizwys.cn/gtesellgqo.html

[U111] JS：对象转 Map
来源：http://hz.52xcode.cn/gtwglukojl.html

new Map(Object.entries(obj))
来源：http://hz.zhiwuduotai.top/gtqqusyxak.html

[U112] JS：字符串补位
来源：http://hz.hywenlv.cn/gtqomssxym.html

"7".padStart(3, "0")
来源：http://hz.havefunace.top/gtqkquibrj.html

[U113] JS：正则替换全部
来源：http://hz.quarkkingdee.top/gtvmiupvbv.html

s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtkayulire.html

[U114] JS：JSON 深比较
来源：http://hz.guannengcc.top/gtmzrwmgne.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtvbpzejhw.html

[U115] JS：生成 UUID
来源：http://hz.cdnleiting.top/gtuosvwbxj.html

crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtocwiyhov.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtggojzmra.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtcpudyfer.html

[U117] JS：单元测试
来源：http://hz.nwbrower.top/gtpjhuqtbh.html

npm i -D vitest;  npx vitest
来源：http://hz.yangfankeji.com/gtophxoyld.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gteyfoqihj.html

npm i -D vite;  npx vite
来源：http://hz.hysaishi.cn/gtpgglphwf.html

[U119] JS：生产构建
来源：http://hz.zhixingplan.top/gtmnrqhbou.html

npx vite build
来源：http://hz.cashguo.top/gtefjwqilf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jyoumei.cn/gtvutmtekq.html

import.meta.env.VITE_API_URL
来源：http://hz.jinyuanbaomall.cn/gtkcnjyrpg.html

================================================================================
来源：http://hz.yonumen.top/gtnziazcww.html

统计汇总
来源：http://hz.hnxiangtu.top/gtkfbsceqq.html

================================================================================
来源：http://hz.bjfxy.top/gtqcuxaeor.html

按语言统计（条）：
来源：http://hz.hywenlv.cn/gtcxnvjpsq.html

Python ......... 252
来源：http://hz.hfpthk.cn/gtrobxwkmn.html

PHP ............ 252
来源：http://hz.tian-w.cn/gtosylxmst.html

JavaScript ..... 252
来源：http://hz.jinqigfzy.top/gtjjlavlqb.html

TypeScript ..... 212
来源：http://hz.9152youxi.cn/gtmmczrdla.html

Java ........... 212
来源：http://hz.chenzaomai.com/gtbdaqaejb.html

Go ............. 212
来源：http://hz.yonumen.top/gtvgblzzlj.html

Ruby ........... 212
来源：http://hz.svipenyu.cn/gtadkyfyyz.html

C# ............. 212
来源：http://hz.fengsongda.top/gtesevfhfs.html

C .............. 30
来源：http://hz.hammf.cn/gtdrgetggn.html

C++ ............ 30
来源：http://hz.jinqigufen.top/gtwuxjwbus.html

SQL ............ 90
来源：http://hz.zhaomingkeji.xyz/gtncfnsdke.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtagyovvzr.html

Kotlin ......... 15
来源：http://hz.jinghuilouyu.cn/gtiseywvgf.html

Swift .......... 15
来源：http://hz.ehwqpu.com/gtpphvrkog.html

Lua ............ 10
来源：http://hz.smart0.xyz/gtwwukbfjs.html

Perl ........... 10
来源：http://hz.zdqjudy.top/gtiquijggv.html

Scala .......... 10
来源：http://hz.cheryme.top/gttcoxgfqu.html

------------------------------------
来源：http://hz.cashguo.top/gtnxwtksya.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gtxqzlvmgf.html

按章节统计：
来源：http://hz.smart0.xyz/gtbjoqgsss.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hywenlv.cn/gtidvjgztq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtucygleaq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtgbidwsko.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtduoexopz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yanxiufei.cn/gtiblljvpx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xingfuxueyuan.xyz/gtewwgcbqt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtkncbfzbx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtaupuomqt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtknupuwru.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.dashuyun.cn/gtvrciumzf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtqhbnbdrc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtyhfcpcgk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtlnmdbige.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtrajonnpl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhoulong.xyz/gtnmlkxbxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtqipplifz.html

Q SQL 专题                              90
来源：http://hz.yuanzhike.top/gtnoszuxih.html

R Bash 专题                             80
来源：http://hz.nanxuanxn.top/gtfvnndhwn.html

S C / C++ 专题                          60
来源：http://hz.ybcxt.top/gtjrewgnek.html

T 其他语言补充                          60
来源：http://hz.chenlongwang.top/gteydydrhz.html

U 高频实用片段                         120
来源：http://hz.fzhhl.top/gtkriwfhna.html

------------------------------------
来源：http://hz.gzhubu.top/gtvtgmrkhi.html

合计                                  2106 条
来源：http://hz.smart0.xyz/gtcjoedikt.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtyfrcmlbg.html

使用提醒
来源：http://hz.svipenyu.cn/gtkgkoqoxj.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gttvvfohqj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gaohongyu789.top/gtjvzmipbo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhijiandao.cn/gtjegqgeel.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.aibaodan.cn/gtyeaubrsg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xziqi.cn/gtdzrlttgo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ywan-chungtsiang.top/gtwaxscazr.html

—— 文件结束 ——
来源：http://hz.hysaishi.cn/gtlfjyzxhx.html

================================================================================
来源：http://hz.ybcxt.top/gthofdjzbb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ybcxt.top/gtrasutuss.html

Common Programming Examples Cheat Book
来源：http://hz.mhx1999.top/gtcambjcpa.html

================================================================================
来源：http://hz.yj20258888.top/gtqvcbdbxb.html

【收录内容】
来源：http://hz.gaohongyu789.top/gtsugwsjqq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtruzeutij.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.snrcjt.cn/gtwnqmopwi.html

SQL · Bash · C · C++
来源：http://hz.52xcode.cn/gtdlbwqdbn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtgsuwrygh.html

【使用说明】
来源：http://hz.ehwqpu.com/gtjmkezvve.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.c1oappe.top/gthlknmpya.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gogol.net.cn/gtzsfcespk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yongpay.top/gtuwlctveb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yj202588.top/gthjccomyy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtrskwpogf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tanke756.top/gtvzowzesl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xuetiantiany.cn/gtuyktfxca.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zycfv.cn/gtqqoyawcg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cqqwz.cn/gtbmnhmbog.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangshuangyany.cn/gtxvkvjtru.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xingfuxueyuan.xyz/gtfaqpbbgg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shuidangran.top/gtyybcoyyi.html

【文件统计】
来源：http://hz.sweek.top/gtzsybamzj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxinkj.top/gtbbtzwisf.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gteeihnkes.html

目  录
来源：http://hz.hywenlv.cn/gtdxictdgu.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtjwbwbhrd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtpzjezqjf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gzhubu.top/gtjfeayzzw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtlarwlltb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yonumen.top/gtrqkftrox.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dashuyun.cn/gtdcqawsoz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jqgfzy.top/gtadbabofr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gturtvjxdj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtyifhlgpt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtzrykhvob.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtvsdtaktl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.fzhhl.top/gthssqpdjq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtfweosvlh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtlyulduwe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.pycfn.com/gtwhlubxyd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xingfuxueyuan.xyz/gtqbuhiryg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtafhicbhs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ywan-chungtsiang.top/gtcsvezdbc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.nwbrower.top/gtulyeunyq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.52xcode.cn/gtgeqkbyhk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtkfqitudt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangkeji.top/gtnluyfugm.html

================================================================================
来源：http://hz.hfpthk.cn/gtqpxqjorf.html

A. 基础语法与类型
来源：http://hz.zhoulong.xyz/gtweqxrihf.html

================================================================================
来源：http://hz.yongpay.top/gtsohgvwjg.html

[A01] Hello World
来源：http://hz.chenlongwang.top/gtyltgcpia.html

Py:   print("Hello, World!")
来源：http://hz.xinyue.icu/gtuxqpwelw.html

PHP:  echo "Hello, World!";
来源：http://hz.hongshengwenyu.top/gtpyffwuoi.html

JS:   console.log("Hello, World!");
来源：http://hz.zhengqikj.top/gtkgqfmulq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.kuanghao11.cn/gtfqrroyen.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtuaoiaweb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtfgtdwsfp.html

Ruby: puts "Hello, World!"
来源：http://hz.hywenlv.cn/gtibckhhyl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.birdmap.top/gtkqoowqdt.html

[A02] 变量声明与赋值
来源：http://hz.hysaishi.cn/gtrmrijpog.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ivvv.top/gtdlwrieew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.dashuyun.cn/gtjlvplxka.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hfpthk.cn/gthwsjoamw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hfpthk.cn/gtnptblunx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cucudq.cn/gtcznfiwgt.html

Go:   name := "Alex"; age := 20
来源：http://hz.iojbl.cn/gtvnjzrvtl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhiwuduotai.top/gtjsqnufpd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xylfe.cn/gtkpbajwqu.html

[A03] 常量定义
来源：http://hz.dashuyun.cn/gthrgjcgnp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aizwys.cn/gtsayludei.html

PHP:  const PI = 3.14159;
来源：http://hz.shuidangran.top/gtdbpftxbr.html

JS:   const PI = 3.14159;
来源：http://hz.ehwqpu.com/gtputfeakp.html

TS:   const PI: number = 3.14159;
来源：http://hz.wangshuangyany.cn/gtxihxmetn.html

Java: static final double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtkchgvrun.html

Go:   const PI = 3.14159
来源：http://hz.yuxming.cn/gtsjzwptfj.html

Ruby: PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtbofreeix.html

C#:   const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtweufvhoh.html

[A04] 判断变量类型
来源：http://hz.jinyuanbaomall.cn/gtxljcivga.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ydjk.org.cn/gtujrbrgrh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.smart0.xyz/gtivrztucb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xuanzx.com/gtrtfprana.html

TS:   typeof x; x instanceof Date
来源：http://hz.sweek.top/gtpftjuxjt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gtkbuoneut.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hywenlv.cn/gtcerrebbs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hongshengwenyu.top/gtluxdqryf.html

C#:   x.GetType().Name; x is int
来源：http://hz.iojbl.cn/gtiqzfihtn.html

[A05] 整数除法与取模
来源：http://hz.pengpengdd.cyou/gtuoguyppf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.quarkkingdee.top/gttwrxlmxc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hammf.cn/gtbemdtjgt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtxfptgrla.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtiltncpfd.html


<!-- 参考信息 -->