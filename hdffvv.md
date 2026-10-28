代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.cheryme.top/gtjmprtjou.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtgjyzksct.html

[U46] PHP：可空类型
来源：http://hz.daria6918.cn/gtlzrmdsde.html

?string $name = null
来源：http://hz.shangyingyoupin.top/gtxlxpynzn.html

[U47] PHP：联合类型
来源：http://hz.xuetiantiany.cn/gtqxvtbeex.html

int|string $id
来源：http://hz.cqqwz.cn/gtybtyzbaf.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtssmsrror.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtvzilahds.html

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gtqhdtilwp.html

public readonly string $name
来源：http://hz.yj20258888.top/gtpubaaccu.html

[U50] PHP：构造器属性提升
来源：http://hz.tian-w.cn/gtwxvhyspm.html

public function __construct(private int $id) {}
来源：http://hz.pycfn.com/gtjitjdueg.html

[U51] PHP：数组解构
来源：http://hz.chenzaomai.com/gtqhcpysma.html

[$a, $b] = $arr;
来源：http://hz.sweek.top/gtmlbaqnrh.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtvsoqyvlz.html

$double = fn($x) => $x * 2;
来源：http://hz.yuxming.cn/gtssiqlnlp.html

[U53] PHP：空合并运算符
来源：http://hz.xylfe.cn/gtmtgwbohw.html

$v = $a ?? $b ?? "default";
来源：http://hz.cdnleiting.top/gtzxjxsxui.html

[U54] PHP：空安全调用
来源：http://hz.gotoacloud.top/gtqxmszevs.html

$obj?->method()
来源：http://hz.zdqjudy.top/gtttkaroig.html

[U55] PHP：match 表达式
来源：http://hz.yueranfly.top/gteuumbsrl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuanzx.com/gtxatudnnl.html

[U56] PHP：命名参数
来源：http://hz.snrcjt.cn/gttokznknm.html

f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtzbfrdsug.html

[U57] PHP：字符串插值
来源：http://hz.tanke756.top/gtwrdhoqcw.html

"值: {$a}"
来源：http://hz.jianghu66.top/gtiplkexft.html

[U58] PHP：数组三件套
来源：http://hz.cashguo.top/gtnfonsodm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sxryk.cn/gtoewrcxva.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtikrbfssx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtsriosrfv.html

[U60] PHP：JSON 编解码
来源：http://hz.dashuyun.cn/gtlmciewer.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ppjwa.cn/gttedvvxzi.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtfaqakile.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtjpflmaje.html

[U62] PHP：日期对象
来源：http://hz.kuanghao11.cn/gtuducocwp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sysykeji.top/gtaddejfoa.html

[U63] PHP：文件读写
来源：http://hz.sxryk.cn/gtkgatwves.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgfzy.top/gtpustjhge.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtsoswvqkq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jlsjyb.cn/gtnwcfxpyc.html

[U65] PHP：会话
来源：http://hz.yj20258888.top/gtojaxxord.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.snrcjt.cn/gtnhddgacw.html

[U66] PHP：设置 Cookie
来源：http://hz.jinghuilouyu.cn/gtnfuyucqh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tianlin.xyz/gtafkbeaax.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gttagbzeiv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gotoacloud.top/gtwuknncyr.html

[U68] PHP：PDO 连接
来源：http://hz.tian-w.cn/gtanxggwru.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xinyue.icu/gtkhlowgco.html

[U69] PHP：PDO 预处理
来源：http://hz.yuanzhike.top/gtpyrcptgy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hammf.cn/gtcijzawph.html

[U70] PHP：PDO 事务
来源：http://hz.jyoumei.cn/gttmsfyghn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ppjwa.cn/gtwsyolbsb.html

[U71] PHP：抛出异常
来源：http://hz.cashguo.top/gttrqhmtco.html

throw new RuntimeException("失败", 500);
来源：http://hz.iojbl.cn/gtdbgvyorv.html

[U72] PHP：写错误日志
来源：http://hz.xingfuxueyuan.xyz/gtmrhfndqm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenjidiqi.icu/gtmypcwxkm.html

[U73] PHP：读取 ini 配置
来源：http://hz.birdmap.top/gtwgqumaho.html

parse_ini_file("config.ini", true)
来源：http://hz.jqgfzy.top/gtbcfzymgg.html

[U74] PHP：读取环境变量
来源：http://hz.redwolf501.top/gtfypsbivm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.52xcode.cn/gtibcyiqpa.html

[U75] PHP：依赖注入
来源：http://hz.jinqigufen.top/gtujdivzue.html

composer require psr/container
来源：http://hz.316326.xyz/gtvnahmhee.html

[U76] PHP：简单路由
来源：http://hz.daxiang520.top/gtxwirimgz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tianlin.xyz/gtywplsnlb.html

[U77] PHP：模板渲染
来源：http://hz.zhongyouzk.top/gtfmyztclk.html

composer require twig/twig
来源：http://hz.birdmap.top/gtbzgqtoah.html

[U78] PHP：单元测试
来源：http://hz.ppjwa.cn/gtivpcxfmr.html

composer require --dev phpunit/phpunit
来源：http://hz.shzxlz.cn/gtvilxlbkr.html

[U79] PHP：静态分析
来源：http://hz.hfpthk.cn/gtsbixmjze.html

composer require --dev phpstan/phpstan
来源：http://hz.dianchejie.cn/gtqokbbtsy.html

[U80] PHP：代码规范修复
来源：http://hz.shangyingyoupin.top/gtnbwauwsv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xingfuxueyuan.xyz/gtvvjviaea.html

[U81] JS：初始化项目
来源：http://hz.zhongyouzk.top/gtyffratam.html

npm init -y;  npm i express
来源：http://hz.jiagoushi.top/gtnzolyukj.html

[U82] JS：package.json 脚本
来源：http://hz.ywan-chungtsiang.top/gtslbwiswz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhiwuduotai.top/gtliybzypf.html

[U83] JS：ES Module 导入导出
来源：http://hz.hnxiangtu.top/gtlcjlgwxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gaohongyu789.top/gtlgjqoban.html

[U84] JS：CommonJS 写法
来源：http://hz.chenjidiqi.icu/gtfdfugokp.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhoulong.xyz/gtgjgqdxrf.html

[U85] JS：可选链
来源：http://hz.jlsjyb.cn/gtgpqtouoy.html

a?.b?.c
来源：http://hz.yj20258888.top/gtbiisidqo.html

[U86] JS：空值合并
来源：http://hz.hfpthk.cn/gtdoemxsxd.html

a ?? b
来源：http://hz.jinqigfzy.top/gtnmrjmpon.html

[U87] JS：解构默认值
来源：http://hz.tianlin.xyz/gtwkgewfzj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.vqdsnc.cn/gtftadrqhb.html

[U88] JS：对象展开合并
来源：http://hz.yueranfly.top/gtyoymtohn.html

{ ...a, ...b }
来源：http://hz.yj202588.top/gtevanazrk.html

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtsyhmmzjd.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtjgsadtoi.html

[U90] JS：数字数组排序
来源：http://hz.zhoulong.xyz/gtoaelfbes.html

[...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtpfxurmss.html

[U91] JS：对象键值遍历
来源：http://hz.aizwys.cn/gtlvccppgu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.aizwys.cn/gtvbmqdjae.html

[U92] JS：深拷贝
来源：http://hz.ydjk.org.cn/gtoqsnigrz.html

structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtnagrghjl.html

[U93] JS：模板字符串
来源：http://hz.ydzc1.top/gtrfwxtjbf.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtmhiurdff.html

[U94] JS：箭头函数
来源：http://hz.havefunace.top/gtxrhhcfoe.html

const double = x => x * 2;
来源：http://hz.nwbrower.top/gtpgfvglwv.html

[U95] JS：Promise 包装
来源：http://hz.jinghuilouyu.cn/gtjujduguh.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gtcfqocskn.html

[U96] JS：async/await 与异常
来源：http://hz.nanxuanxn.top/gtvvxduryq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtuahnpoew.html

[U97] JS：并发请求
来源：http://hz.quarkkingdee.top/gtastzawxh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gthahfxlyg.html

[U98] JS：fetch 带 JSON
来源：http://hz.cdnleiting.top/gtdnpkmnel.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yanxiufei.cn/gtomydizvz.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtsizxeqmr.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtfjhahhrk.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtitrhwgys.html

document.querySelector(".item")
来源：http://hz.hongshengwenyu.top/gtwgtvjvfx.html

[U101] JS：classList 操作
来源：http://hz.havefunace.top/gtznhmmzua.html

el.classList.toggle("active")
来源：http://hz.yj20258.top/gtbzprlfty.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gtbyojxedx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.smart0.xyz/gtwkcgzecf.html

[U103] JS：定时器
来源：http://hz.snrcjt.cn/gtzxpneptg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.316326.xyz/gtyssmexlg.html

[U104] JS：防抖
来源：http://hz.zhongyouzk.top/gtsojfbocp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtenuyubxw.html

[U105] JS：节流
来源：http://hz.jlsjyb.cn/gtiwugmcwh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jlsjyb.cn/gtcdpqolea.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtqbuqsjdj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cucudq.cn/gthwpekoji.html

[U107] JS：数字千分位
来源：http://hz.zhiwuduotai.top/gtxtrmcgzh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cdnleiting.top/gtxxoovvit.html

[U108] JS：随机整数
来源：http://hz.sweek.top/gtxpkfgbfg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.andypj.xyz/gtbyjhwitz.html

[U109] JS：数组分组
来源：http://hz.9152youxi.cn/gtnxcgdeko.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gttkmflvry.html

[U110] JS：数组分块
来源：http://hz.ehwqpu.com/gtdbegrhir.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258.top/gtfgfufdzi.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangkeji.top/gtuugygpbu.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtbfiwzqfs.html

[U112] JS：字符串补位
来源：http://hz.fengsongda.top/gtxyxyrjaw.html

"7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtqalrbnmj.html

[U113] JS：正则替换全部
来源：http://hz.dashuyun.cn/gtoliqivet.html

s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtpkutmewe.html

[U114] JS：JSON 深比较
来源：http://hz.chenjidiqi.icu/gtuhkfpkhn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtvgbwotgq.html

[U115] JS：生成 UUID
来源：http://hz.yvedp.cn/gtssatidiy.html

crypto.randomUUID()
来源：http://hz.cdnleiting.top/gthoimnntd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sufxvd.cn/gtsrqkrsll.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tian-w.cn/gtcsstjpfb.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtkkxfypcd.html

npm i -D vitest;  npx vitest
来源：http://hz.redwolf501.top/gtwfgfqudu.html

[U118] JS：开发服务器
来源：http://hz.ppjwa.cn/gtazebqscg.html

npm i -D vite;  npx vite
来源：http://hz.ywan-chungtsiang.top/gtyjxotpod.html

[U119] JS：生产构建
来源：http://hz.sysykeji.top/gtifuxfwjo.html

npx vite build
来源：http://hz.hywenlv.cn/gtogdciurv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nanxuanxn.top/gtrqxmcqco.html

import.meta.env.VITE_API_URL
来源：http://hz.yuanzhike.top/gtbgzhsgst.html

================================================================================
来源：http://hz.yj202588.top/gtyugietrl.html

统计汇总
来源：http://hz.vqdsnc.cn/gtmkttyywk.html

================================================================================
来源：http://hz.nwbrower.top/gtziyrjrvl.html

按语言统计（条）：
来源：http://hz.cashguo.top/gtwmzpcwzw.html

Python ......... 252
来源：http://hz.zhijiandao.cn/gtnonxdegz.html

PHP ............ 252
来源：http://hz.zhaomingkeji.xyz/gtxolpyzbl.html

JavaScript ..... 252
来源：http://hz.xuetiantiany.cn/gtscjxzkvj.html

TypeScript ..... 212
来源：http://hz.jinghuilouyu.cn/gtxyobnylu.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtbvwxyljh.html

Go ............. 212
来源：http://hz.ydjk.org.cn/gtofzboutl.html

Ruby ........... 212
来源：http://hz.0kj1m.cn/gtsfankzou.html

C# ............. 212
来源：http://hz.aibaodan.cn/gtjicpnser.html

C .............. 30
来源：http://hz.snrcjt.cn/gtaldvhtja.html

C++ ............ 30
来源：http://hz.ehwqpu.com/gtjbbdrlzl.html

SQL ............ 90
来源：http://hz.jyoumei.cn/gtherpsazm.html

Bash ........... 80
来源：http://hz.pengpengdd.cyou/gtbxgmricd.html

Kotlin ......... 15
来源：http://hz.aibaodan.cn/gtfusezwsc.html

Swift .......... 15
来源：http://hz.zhaomingkeji.xyz/gtjeipayev.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gtqetrhshs.html

Perl ........... 10
来源：http://hz.smart0.xyz/gtilbwacui.html

Scala .......... 10
来源：http://hz.tanke756.top/gtpmnhbcui.html

------------------------------------
来源：http://hz.316326.xyz/gtogeljlnq.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gtscjhwoxn.html

按章节统计：
来源：http://hz.52xcode.cn/gtotlbwvpf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.redwolf501.top/gttpawtqwo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.0kj1m.cn/gtcdppziih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gotoacloud.top/gtjntckdal.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gtqtfsppwj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jqgufenzy.top/gtdlahxcgc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtrbwnflpr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gttoujtvqn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtwpaiglnl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtnphrqddt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtaorsjemh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtpqdvjndm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtrvnaqfzy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cdnleiting.top/gtpbtygpaw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtdthieyrf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daria6918.cn/gtzinhgkag.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtotfixtpu.html

Q SQL 专题                              90
来源：http://hz.gotoacloud.top/gttknxklic.html

R Bash 专题                             80
来源：http://hz.aizwys.cn/gtellcnsvl.html

S C / C++ 专题                          60
来源：http://hz.zhongyouzk.top/gtdcnurond.html

T 其他语言补充                          60
来源：http://hz.fengsongda.top/gtiawvrihn.html

U 高频实用片段                         120
来源：http://hz.haohaochexian.top/gthzxxkdmt.html

------------------------------------
来源：http://hz.52xcode.cn/gtlwnbqhvb.html

合计                                  2106 条
来源：http://hz.zhaomingkeji.xyz/gtopdlvflm.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtspyyunms.html

使用提醒
来源：http://hz.sxryk.cn/gtjmdzgfrg.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtukwqgrjj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtcgdaoubq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tanke756.top/gtnjelughz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yangfankeji.com/gtpfpceeme.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jyoumei.cn/gtbkqjsqmk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xziqi.cn/gtpqgjvwwt.html

—— 文件结束 ——
来源：http://hz.yongpay.top/gtveqqlqtu.html

================================================================================
来源：http://hz.zhixingplan.top/gtewvwbzyx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.redwolf501.top/gtatwjeokg.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigfzy.top/gttelipzrn.html

================================================================================
来源：http://hz.daxiang520.top/gtzybspjva.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtsvwrwmej.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cdnleiting.top/gtmvekhlqg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtbkufdvmw.html

SQL · Bash · C · C++
来源：http://hz.jianghu66.top/gtslpruxgq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhijiandao.cn/gtehbeicam.html

【使用说明】
来源：http://hz.zhoulong.xyz/gttmlpcvgq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.pycfn.com/gtgomrouee.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yanxiufei.cn/gtrnsuxmeb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xziqi.cn/gtosaxsgyo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.nanxuanxn.top/gtsbhfmlra.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.bjfxy.top/gtlxnklmyi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xylfe.cn/gtilbqefjg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.fzhhl.top/gtroskjvhb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhengqikj.top/gtroazudvz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.0kj1m.cn/gtsuuvebzd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.aizwys.cn/gtpgxlhmoy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sysykeji.top/gtjkfecahc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhijiandao.cn/gthnzqbhya.html

【文件统计】
来源：http://hz.andypj.xyz/gtdxuxxabg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tianlin.xyz/gtjcxhsfug.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtluhredze.html

目  录
来源：http://hz.xinyue.icu/gtwntfqnth.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtxixxsckb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yvedp.cn/gtqdpphxii.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtdotizeka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtiazcyvnk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtotijsrwz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgufenzy.top/gtbpasuhke.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.daria6918.cn/gtwoiphlur.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.0kj1m.cn/gtjpsgrczi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtkebxybfh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtpcyxlece.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtaykmhcfx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtbxmvjcvr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtqvmsnjbo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtlteaktbb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zdqjudy.top/gthuptdzxi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.guowangkeji.top/gtfyrvamrz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtzpsjcixm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.feifeiyinyue.top/gtvymrcwnh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sxryk.cn/gtepezjlbh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zdqjudy.top/gttklcoqwk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtoafqhxbp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.haohaochexian.top/gtwujcgtar.html

================================================================================
来源：http://hz.dashuyun.cn/gttgbviupd.html

A. 基础语法与类型
来源：http://hz.kuanghao11.cn/gtvhvyccll.html

================================================================================
来源：http://hz.sweek.top/gtipotzfkb.html

[A01] Hello World
来源：http://hz.fengsongda.top/gtqmflumau.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtusmdhybh.html

PHP:  echo "Hello, World!";
来源：http://hz.52xcode.cn/gtnwoummsi.html

JS:   console.log("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtqmyjpopu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.iojbl.cn/gtseeavugs.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj202588.top/gtohcvckyr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yuanzhike.top/gtzqyjmzrx.html

Ruby: puts "Hello, World!"
来源：http://hz.ppjwa.cn/gtvluisnpv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangdashe.top/gtzpzjmage.html

[A02] 变量声明与赋值
来源：http://hz.hywenlv.cn/gtzywekpcj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.redwolf501.top/gthpufegls.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gteapdlewr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.nwbrower.top/gthktxreqt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ivvv.top/gtpleditjr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gthrihgayx.html

Go:   name := "Alex"; age := 20
来源：http://hz.ydzc1.top/gtlojrwryb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xylfe.cn/gtihnprtvz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xziqi.cn/gtwxlhwzbw.html

[A03] 常量定义
来源：http://hz.zhoulong.xyz/gtlltcfque.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sweek.top/gtblxasfsk.html

PHP:  const PI = 3.14159;
来源：http://hz.c1oappe.top/gtawophjnk.html

JS:   const PI = 3.14159;
来源：http://hz.xylfe.cn/gtnnlouezq.html

TS:   const PI: number = 3.14159;
来源：http://hz.yonumen.top/gtysaikmge.html

Java: static final double PI = 3.14159;
来源：http://hz.smart0.xyz/gtushjspuk.html

Go:   const PI = 3.14159
来源：http://hz.jinyuanbaomall.cn/gtdhioqwft.html

Ruby: PI = 3.14159
来源：http://hz.hammf.cn/gtdubsgwqu.html

C#:   const double PI = 3.14159;
来源：http://hz.xinyue.icu/gthdnjcbne.html

[A04] 判断变量类型
来源：http://hz.fengsongda.top/gtvbahhhwp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.fengsongda.top/gtetonccfb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guannengcc.top/gtwacddxox.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.9152youxi.cn/gtjirbucta.html

TS:   typeof x; x instanceof Date
来源：http://hz.andypj.xyz/gtvqyioksh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yueranfly.top/gtrhpteqir.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cashguo.top/gtulnhiiec.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.fengsongda.top/gtxmpidhli.html

C#:   x.GetType().Name; x is int
来源：http://hz.fengsongda.top/gtfdcwcqng.html

[A05] 整数除法与取模
来源：http://hz.guowangkeji.top/gtfmbfcdbl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.mhx1999.top/gtgosctjpd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtjcoqtxva.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ydzc1.top/gtbooqkgaq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.snrcjt.cn/gtylyissuo.html


<!-- 参考信息 -->