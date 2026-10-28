代发 wailian999

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtwhrqzair.html

int|string $id
来源：http://hz.sysykeji.top/gtlikipmjz.html

[U48] PHP：纯枚举
来源：http://hz.fengsongda.top/gtdtahnwct.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cdnleiting.top/gthefchhgx.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtrqeczqfm.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtcmpioquk.html

[U50] PHP：构造器属性提升
来源：http://hz.316326.xyz/gtigqgelwz.html

public function __construct(private int $id) {}
来源：http://hz.andypj.xyz/gtxqebhslp.html

[U51] PHP：数组解构
来源：http://hz.316326.xyz/gtuenvfygb.html

[$a, $b] = $arr;
来源：http://hz.ybcxt.top/gtssiqaqmr.html

[U52] PHP：箭头函数
来源：http://hz.cucudq.cn/gtkrudwmgg.html

$double = fn($x) => $x * 2;
来源：http://hz.hammf.cn/gtbtdvkwat.html

[U53] PHP：空合并运算符
来源：http://hz.guannengcc.top/gtnoxwbgfk.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gtsjrtjhkz.html

[U54] PHP：空安全调用
来源：http://hz.daxiang520.top/gtdgrendqp.html

$obj?->method()
来源：http://hz.shzxlz.cn/gtiurtmdyz.html

[U55] PHP：match 表达式
来源：http://hz.dashuyun.cn/gtuwlhrmcb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cucudq.cn/gtklmwdpsq.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtnphwiacv.html

f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtdexggpsm.html

[U57] PHP：字符串插值
来源：http://hz.kuanghao11.cn/gtzjeosart.html

"值: {$a}"
来源：http://hz.chenjidiqi.icu/gtqwhtjggg.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtajkrudwa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.guowangkeji.top/gtisbjjthd.html

[U59] PHP：自定义排序
来源：http://hz.meibo888.top/gtpngfdkiu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtqxkqgjuf.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgfzy.top/gtpmvjztvr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuetiantiany.cn/gtpzbakqxw.html

[U61] PHP：正则
来源：http://hz.yuanzhike.top/gtnwsunynm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtebofsydx.html

[U62] PHP：日期对象
来源：http://hz.hnqzz.top/gtegrpqcfj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.pycfn.com/gtxbxcvlrc.html

[U63] PHP：文件读写
来源：http://hz.hywenlv.cn/gtzkqmpwfs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangtech.top/gtgtoenwfd.html

[U64] PHP：目录遍历
来源：http://hz.jiagoushi.top/gtomvdqdws.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tian-w.cn/gtdplhsuqy.html

[U65] PHP：会话
来源：http://hz.ehwqpu.com/gtnaxtdyff.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.316326.xyz/gtsyqfblqu.html

[U66] PHP：设置 Cookie
来源：http://hz.yuxming.cn/gtkgvmezqi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hywenlv.cn/gtdipawcry.html

[U67] PHP：处理文件上传
来源：http://hz.sufxvd.cn/gtoivbjpkw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aibaodan.cn/gttycyxvsi.html

[U68] PHP：PDO 连接
来源：http://hz.shanyushiyangtech.top/gtlpwwclmj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.birdmap.top/gtzpgsduvt.html

[U69] PHP：PDO 预处理
来源：http://hz.jinqigufen.top/gttqndgvch.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gtiqntjvcv.html

[U70] PHP：PDO 事务
来源：http://hz.aibaodan.cn/gtsbjusvyp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhixingplan.top/gtvqldapqv.html

[U71] PHP：抛出异常
来源：http://hz.shuidangran.top/gttmkrtdob.html

throw new RuntimeException("失败", 500);
来源：http://hz.yongpay.top/gtumoqstxh.html

[U72] PHP：写错误日志
来源：http://hz.zdqjudy.top/gtaranptxk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xuetiantiany.cn/gtzndousod.html

[U73] PHP：读取 ini 配置
来源：http://hz.xuetiantiany.cn/gtiymuqhsl.html

parse_ini_file("config.ini", true)
来源：http://hz.zdqjudy.top/gtjuxyyijl.html

[U74] PHP：读取环境变量
来源：http://hz.sweek.top/gtbcszygmy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.daxiang520.top/gtdexmeskc.html

[U75] PHP：依赖注入
来源：http://hz.gogol.net.cn/gtvhiwsmoq.html

composer require psr/container
来源：http://hz.zhixingplan.top/gtfdtwzefd.html

[U76] PHP：简单路由
来源：http://hz.smart0.xyz/gtlrruifdo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xylfe.cn/gtsmxiyeuz.html

[U77] PHP：模板渲染
来源：http://hz.haohaochexian.top/gtdncbdzdf.html

composer require twig/twig
来源：http://hz.52xcode.cn/gttgnwibcl.html

[U78] PHP：单元测试
来源：http://hz.zhengqikj.top/gtofihjfqj.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigufen.top/gtcslwndyl.html

[U79] PHP：静态分析
来源：http://hz.cucudq.cn/gteoyfqerm.html

composer require --dev phpstan/phpstan
来源：http://hz.ivvv.top/gtmjfqimkj.html

[U80] PHP：代码规范修复
来源：http://hz.zhiwuduotai.top/gtvxgepeho.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yvedp.cn/gtlkuqfryi.html

[U81] JS：初始化项目
来源：http://hz.daria6918.cn/gtshiqtatp.html

npm init -y;  npm i express
来源：http://hz.nanxinkj.top/gtvjbsyqdk.html

[U82] JS：package.json 脚本
来源：http://hz.sweek.top/gtevorfjxe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cucudq.cn/gtayalgczz.html

[U83] JS：ES Module 导入导出
来源：http://hz.dashuyun.cn/gtwxlkqyxw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhoulong.xyz/gtmvahulre.html

[U84] JS：CommonJS 写法
来源：http://hz.ivvv.top/gtrwdwqaqq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cdnleiting.top/gtregmtsdp.html

[U85] JS：可选链
来源：http://hz.52xcode.cn/gtmtesivwn.html

a?.b?.c
来源：http://hz.feifeiyinyue.top/gtwhfyktow.html

[U86] JS：空值合并
来源：http://hz.smart0.xyz/gtqaiztiyl.html

a ?? b
来源：http://hz.nanxinkj.top/gtfyksptzv.html

[U87] JS：解构默认值
来源：http://hz.fzhhl.top/gtqvfjmbth.html

const { a = 1, b = 2 } = obj;
来源：http://hz.dianchejie.cn/gtlwodynsr.html

[U88] JS：对象展开合并
来源：http://hz.yj20258.top/gtwtlesixj.html

{ ...a, ...b }
来源：http://hz.aizwys.cn/gtftureqzo.html

[U89] JS：数组去重
来源：http://hz.yangfankeji.com/gtoybxfnuy.html

[...new Set(arr)]
来源：http://hz.fengsongda.top/gtsnyibcph.html

[U90] JS：数字数组排序
来源：http://hz.snrcjt.cn/gtvtafcqqh.html

[...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtrlsmyqrk.html

[U91] JS：对象键值遍历
来源：http://hz.haohaochexian.top/gtgpnvuags.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jiagoushi.top/gtmayytmqs.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gthitqsrxt.html

structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtlcawfaqz.html

[U93] JS：模板字符串
来源：http://hz.wangdashe.top/gtbypdeuqp.html

`共 ${n} 条`
来源：http://hz.cqqwz.cn/gtqrzizbgu.html

[U94] JS：箭头函数
来源：http://hz.shanyushiyangtech.top/gtrlfcyykm.html

const double = x => x * 2;
来源：http://hz.52xcode.cn/gtwikolpeu.html

[U95] JS：Promise 包装
来源：http://hz.vqdsnc.cn/gtdksixkgw.html

new Promise((resolve, reject) => {})
来源：http://hz.gogol.net.cn/gtocbqnpae.html

[U96] JS：async/await 与异常
来源：http://hz.zdqjudy.top/gtolsapysx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtzkfkjmir.html

[U97] JS：并发请求
来源：http://hz.cqqwz.cn/gtxaxsvgnw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtccmobcpr.html

[U98] JS：fetch 带 JSON
来源：http://hz.xuetiantiany.cn/gtgldkfpid.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.fzhhl.top/gtiltuxaxq.html

[U99] JS：事件监听
来源：http://hz.xingfuxueyuan.xyz/gtefvskswk.html

el.addEventListener("click", e => {})
来源：http://hz.xziqi.cn/gtsuqwocls.html

[U100] JS：DOM 查询
来源：http://hz.xuanzx.com/gttwmzfowk.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtgcfjyjlh.html

[U101] JS：classList 操作
来源：http://hz.gzhubu.top/gtkaagliih.html

el.classList.toggle("active")
来源：http://hz.xuanzx.com/gtconiuawn.html

[U102] JS：本地存储
来源：http://hz.zhongyouzk.top/gtgxkdeifk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gtsasfikkl.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtjvfcdxji.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sufxvd.cn/gtbakggqte.html

[U104] JS：防抖
来源：http://hz.iojbl.cn/gtsgaqmnku.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtnpadtbjl.html

[U105] JS：节流
来源：http://hz.sweek.top/gtoydhzqzc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuxming.cn/gtkrrpxrhp.html

[U106] JS：日期格式化
来源：http://hz.zhixingplan.top/gthvymwxhq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zycfv.cn/gticonnzad.html

[U107] JS：数字千分位
来源：http://hz.havefunace.top/gtwqxtyqcr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgfzy.top/gtfoqmvozi.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtyzsmvccq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gthprojjzh.html

[U109] JS：数组分组
来源：http://hz.shanyushiyangtech.top/gtdnznltwv.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtnpvzfoqv.html

[U110] JS：数组分块
来源：http://hz.sufxvd.cn/gtpkmfbokn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gzhubu.top/gtndetodbw.html

[U111] JS：对象转 Map
来源：http://hz.ydzc1.top/gthfgbayhp.html

new Map(Object.entries(obj))
来源：http://hz.yuanzhike.top/gthlxcbzox.html

[U112] JS：字符串补位
来源：http://hz.quarkkingdee.top/gtmsmritpm.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtqvevrycm.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gttzijdzqg.html

s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtqfiehqsk.html

[U114] JS：JSON 深比较
来源：http://hz.yvedp.cn/gtkqwrhlmn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtfjpwafpv.html

[U115] JS：生成 UUID
来源：http://hz.yongpay.top/gtrmxzucsv.html

crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtjwibdssx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtesjvvquw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daxiang520.top/gtvlvzsrui.html

[U117] JS：单元测试
来源：http://hz.ybcxt.top/gthpcoofcf.html

npm i -D vitest;  npx vitest
来源：http://hz.tianlin.xyz/gtrilikhni.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtmwxfkfwi.html

npm i -D vite;  npx vite
来源：http://hz.hammf.cn/gtzstdwzjz.html

[U119] JS：生产构建
来源：http://hz.c1oappe.top/gtrnuhdqys.html

npx vite build
来源：http://hz.ydjk.org.cn/gtavnytvym.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hfpthk.cn/gtwoorduso.html

import.meta.env.VITE_API_URL
来源：http://hz.fzhhl.top/gtwddqyxvv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtnwgmsjou.html

统计汇总
来源：http://hz.aizwys.cn/gtnixljsgx.html

================================================================================
来源：http://hz.ydzc1.top/gtxcupisjd.html

按语言统计（条）：
来源：http://hz.hammf.cn/gtxsoedjun.html

Python ......... 252
来源：http://hz.cheryme.top/gtoxzodwop.html

PHP ............ 252
来源：http://hz.guowangkeji.top/gtcjrvkgag.html

JavaScript ..... 252
来源：http://hz.yj20258.top/gtougofsdr.html

TypeScript ..... 212
来源：http://hz.ydjk.org.cn/gtxuespwcm.html

Java ........... 212
来源：http://hz.kuanghao11.cn/gtdobkzumu.html

Go ............. 212
来源：http://hz.havefunace.top/gtdedfdsxd.html

Ruby ........... 212
来源：http://hz.hammf.cn/gtrtqwqrwz.html

C# ............. 212
来源：http://hz.guowangkeji.top/gtluqnubpa.html

C .............. 30
来源：http://hz.ppjwa.cn/gtukjvcxei.html

C++ ............ 30
来源：http://hz.guannengcc.top/gtngczopmz.html

SQL ............ 90
来源：http://hz.snrcjt.cn/gtufchalem.html

Bash ........... 80
来源：http://hz.xuanzx.com/gtakvndexq.html

Kotlin ......... 15
来源：http://hz.ehwqpu.com/gtwlmajgsi.html

Swift .......... 15
来源：http://hz.zdqjudy.top/gtikltvdge.html

Lua ............ 10
来源：http://hz.fengsongda.top/gtefgirxuy.html

Perl ........... 10
来源：http://hz.9152youxi.cn/gtpjhnjexn.html

Scala .......... 10
来源：http://hz.hammf.cn/gtaidnjsgl.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtkzmxyzur.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gtstdobszx.html

按章节统计：
来源：http://hz.nwbrower.top/gtrodcbuuk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtzqpjhujq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zycfv.cn/gtwmcqoeoq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtmqmimfee.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.pengpengdd.cyou/gtjyfunbyd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jlsjyb.cn/gteocupjel.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gtaqwypvfc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gthwqnouen.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtmngesjaw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtptyggqwa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.pengpengdd.cyou/gtepuhtoyr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gtcnelltnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtcngmfkwn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtvohewgbl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.fzhhl.top/gtjefeefqm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hywenlv.cn/gthzzywply.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gthkhicgbx.html

Q SQL 专题                              90
来源：http://hz.hysaishi.cn/gtfcffcbqn.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gthulfwyyo.html

S C / C++ 专题                          60
来源：http://hz.havefunace.top/gtoxklerxo.html

T 其他语言补充                          60
来源：http://hz.yuanzhike.top/gtunfqftpw.html

U 高频实用片段                         120
来源：http://hz.fengsongda.top/gtwhzkghet.html

------------------------------------
来源：http://hz.tian-w.cn/gtmlpluypz.html

合计                                  2106 条
来源：http://hz.jqgufenzy.top/gtgbdrfstf.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtnbbqutbu.html

使用提醒
来源：http://hz.bjfxy.top/gtnahvkvwe.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtizjnjjfi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtygzfpyja.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.wangdashe.top/gtbgucqkup.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sysykeji.top/gtoduaxkhc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ybcxt.top/gtexprlwhu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.nanxinkj.top/gtrlkvxjaa.html

—— 文件结束 ——
来源：http://hz.sufxvd.cn/gtzswmugxt.html

================================================================================
来源：http://hz.zhengqikj.top/gtkrtgevjw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sxryk.cn/gtlwwhryyf.html

Common Programming Examples Cheat Book
来源：http://hz.hnqzz.top/gtstvlwart.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthbqpyakh.html

【收录内容】
来源：http://hz.jinqigfzy.top/gtncotspnr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.9152youxi.cn/gtbmxjsqlb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.smart0.xyz/gtqkjenwck.html

SQL · Bash · C · C++
来源：http://hz.kuanghao11.cn/gtynzbllhi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gogol.net.cn/gtldfvnjid.html

【使用说明】
来源：http://hz.tanke756.top/gtmyrfxjnt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yanxiufei.cn/gtscxedcpg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhongyouzk.top/gtreyzsqsi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yvedp.cn/gteasbqysj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.aizwys.cn/gtrarrspny.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gaohongyu789.top/gttnpldrqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ybcxt.top/gtrsjlldpr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.guannengcc.top/gtrxtibafc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hnxiangtu.top/gtcqaatvys.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xylfe.cn/gtuflbkbvk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.aibaodan.cn/gtuoxgvuhp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gogol.net.cn/gtvyazjrlo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hysaishi.cn/gtfdhtanfy.html

【文件统计】
来源：http://hz.ivvv.top/gtkgfzmcya.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yueranfly.top/gtphitnjne.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtphbssbkg.html

目  录
来源：http://hz.cashguo.top/gtpkwzwkzn.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gthixiqpka.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gttmzufnha.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gtnyjwobnw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jyoumei.cn/gtuqymtddu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtdhzcacrn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cucudq.cn/gtxvkufbez.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jlsjyb.cn/gtelwshpwd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtsfwufyov.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gthdibdija.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtuqyofawq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ybcxt.top/gtpuaqxnfj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhiwuduotai.top/gtcqvpllqg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtltrckxdz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gttzhdgmot.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtnvaeujme.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shzxlz.cn/gtakiofbcw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gogol.net.cn/gtxyqrbtot.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ybcxt.top/gtulhvgcet.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yonumen.top/gtrmfrcuxz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.guowangkeji.top/gtextlnmhw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jianghu66.top/gtoqjouoyo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtzvqoruyc.html

================================================================================
来源：http://hz.yuanzhike.top/gtaszbgtnv.html

A. 基础语法与类型
来源：http://hz.pycfn.com/gtefjsymfw.html

================================================================================
来源：http://hz.yj20258888.top/gtcetmffrq.html

[A01] Hello World
来源：http://hz.dashuyun.cn/gtlbnlrjzw.html

Py:   print("Hello, World!")
来源：http://hz.zhongyouzk.top/gteqevnukg.html

PHP:  echo "Hello, World!";
来源：http://hz.xingfuxueyuan.xyz/gticcqsoqc.html

JS:   console.log("Hello, World!");
来源：http://hz.zhixingplan.top/gtfkqhpxhy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xuetiantiany.cn/gtdwnbbdqx.html

Java: System.out.println("Hello, World!");
来源：http://hz.gaohongyu789.top/gtnonfspug.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.aibaodan.cn/gtztvdijsm.html

Ruby: puts "Hello, World!"
来源：http://hz.316326.xyz/gtguwknzev.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.iojbl.cn/gtmuqeeuyr.html

[A02] 变量声明与赋值
来源：http://hz.dashuyun.cn/gtupljnhgx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cashguo.top/gtniutwfhy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sweek.top/gtdwtrljgg.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenlongwang.top/gtggqbewrr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhoulong.xyz/gtvviuaibg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhaomingkeji.xyz/gtjiifbmng.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenlongwang.top/gtgwqcimpu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yueranfly.top/gtcxzfgkgz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.fengsongda.top/gttnzxnmco.html

[A03] 常量定义
来源：http://hz.aizwys.cn/gtojluhesg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aibaodan.cn/gtzjcqwqzc.html

PHP:  const PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtigrixclb.html

JS:   const PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtxtudvgek.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhiwuduotai.top/gtaoyhkoay.html

Java: static final double PI = 3.14159;
来源：http://hz.c1oappe.top/gtpulotiic.html

Go:   const PI = 3.14159
来源：http://hz.zdqjudy.top/gtslalrcbw.html

Ruby: PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtwrvrtrkr.html

C#:   const double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtdtaapekd.html

[A04] 判断变量类型
来源：http://hz.zhoulong.xyz/gtiauteqjl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.sysykeji.top/gtyfkfwsyg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xuetiantiany.cn/gtzsnrqllp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yonumen.top/gtywyfsfbb.html

TS:   typeof x; x instanceof Date
来源：http://hz.guowangkeji.top/gtyrztoqkr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.aibaodan.cn/gtrqytdkad.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.nanxinkj.top/gtibbjradx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shanyushiyangtech.top/gtiyretnjx.html

C#:   x.GetType().Name; x is int
来源：http://hz.0kj1m.cn/gtfirpdvpn.html

[A05] 整数除法与取模
来源：http://hz.yongpay.top/gtkixewuve.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yj202588.top/gtphwmxqcr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gotoacloud.top/gtpyxnaprv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shuidangran.top/gtqoqwcemk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xziqi.cn/gtbyxosxpl.html

Java: 7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtszgpawdw.html

Go:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtzvetlewv.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtqkvwukvv.html

C#:   7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gthyrlihzn.html


<!-- 参考信息 -->