代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.zycfv.cn/gtaewoydtr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.kuanghao11.cn/gtqtbejqul.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtpsywyxhd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hnqzz.top/gtzalevasf.html

[U43] PHP：声明命名空间
来源：http://hz.zhixingplan.top/gtwozxcdsn.html

namespace App\Http;
来源：http://hz.feifeiyinyue.top/gtellmytvw.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gtptosfoky.html

declare(strict_types=1);
来源：http://hz.ywan-chungtsiang.top/gtmiohnmgb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.mhx1999.top/gtigufuger.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtmwxmqaps.html

[U46] PHP：可空类型
来源：http://hz.xinyue.icu/gtmtxssedt.html

?string $name = null
来源：http://hz.bjfxy.top/gtkgtionbk.html

[U47] PHP：联合类型
来源：http://hz.shangyingyoupin.top/gtebmfzkpn.html

int|string $id
来源：http://hz.zhijiandao.cn/gtpzgeihkm.html

[U48] PHP：纯枚举
来源：http://hz.jinghuilouyu.cn/gtqtztstzh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ppjwa.cn/gtmytqelne.html

[U49] PHP：只读属性
来源：http://hz.yueranfly.top/gtwaqqasza.html

public readonly string $name
来源：http://hz.sysykeji.top/gtnqhtecgj.html

[U50] PHP：构造器属性提升
来源：http://hz.haohaochexian.top/gtdglwqapr.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtxjkmkxaw.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtohknbgkg.html

[$a, $b] = $arr;
来源：http://hz.svipenyu.cn/gtfmuirpit.html

[U52] PHP：箭头函数
来源：http://hz.zhijiandao.cn/gthfhoxdlu.html

$double = fn($x) => $x * 2;
来源：http://hz.fzhhl.top/gtyxttsykc.html

[U53] PHP：空合并运算符
来源：http://hz.iojbl.cn/gtaachzyfw.html

$v = $a ?? $b ?? "default";
来源：http://hz.52xcode.cn/gteqzowtcy.html

[U54] PHP：空安全调用
来源：http://hz.gogol.net.cn/gtxmelrtri.html

$obj?->method()
来源：http://hz.316326.xyz/gtzhcfkkqr.html

[U55] PHP：match 表达式
来源：http://hz.cqqwz.cn/gtiicmbcpj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtgwvunlfg.html

[U56] PHP：命名参数
来源：http://hz.xingfuxueyuan.xyz/gtxirphewp.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtrwznnsuv.html

[U57] PHP：字符串插值
来源：http://hz.tanke756.top/gthqvrxcjh.html

"值: {$a}"
来源：http://hz.shanyushiyangtech.top/gteloydtbu.html

[U58] PHP：数组三件套
来源：http://hz.hammf.cn/gtmicppafs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aizwys.cn/gtmegvxrbw.html

[U59] PHP：自定义排序
来源：http://hz.chenlongwang.top/gtznnspiqf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sufxvd.cn/gtkhyykwop.html

[U60] PHP：JSON 编解码
来源：http://hz.quarkkingdee.top/gtatxanmqe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ybcxt.top/gtvlnizvix.html

[U61] PHP：正则
来源：http://hz.xingfuxueyuan.xyz/gtcvhfqpxc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtvzuyrnch.html

[U62] PHP：日期对象
来源：http://hz.52xcode.cn/gtrttyzhho.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hnxiangtu.top/gtlrxklwsl.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gtgjoxalkh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gaohongyu789.top/gthsrduzhl.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gtpbdakztj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangshuangyany.cn/gtfzfovxfl.html

[U65] PHP：会话
来源：http://hz.zhongyouzk.top/gttnbtcwpj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sysykeji.top/gtiomubqvx.html

[U66] PHP：设置 Cookie
来源：http://hz.chenzaomai.com/gtumthaetk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yanxiufei.cn/gtlrprgkcq.html

[U67] PHP：处理文件上传
来源：http://hz.jinyuanbaomall.cn/gtsqghnoef.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gzhubu.top/gtlklavlha.html

[U68] PHP：PDO 连接
来源：http://hz.mhx1999.top/gtqsyiugoi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.svipenyu.cn/gtpqkqpcwj.html

[U69] PHP：PDO 预处理
来源：http://hz.sxryk.cn/gtefowgcgy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj20258.top/gtakjheodf.html

[U70] PHP：PDO 事务
来源：http://hz.nanxinkj.top/gtwipzgeqi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtotbjpdca.html

[U71] PHP：抛出异常
来源：http://hz.hongshengwenyu.top/gtwodtbbia.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhaomingkeji.xyz/gtkdfjytkz.html

[U72] PHP：写错误日志
来源：http://hz.hywenlv.cn/gtzdwivrkd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.c1oappe.top/gtkbdhrnre.html

[U73] PHP：读取 ini 配置
来源：http://hz.jiagoushi.top/gtkhrntoda.html

parse_ini_file("config.ini", true)
来源：http://hz.xziqi.cn/gtpaxlvbyq.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtfrdafhvg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tianlin.xyz/gtzlbwrdbc.html

[U75] PHP：依赖注入
来源：http://hz.zhaomingkeji.xyz/gtrtauwswq.html

composer require psr/container
来源：http://hz.316326.xyz/gtjhwkdptn.html

[U76] PHP：简单路由
来源：http://hz.sysykeji.top/gtfutxkmps.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinyuanbaomall.cn/gtmgknbtdb.html

[U77] PHP：模板渲染
来源：http://hz.yj202588.top/gtkqxhrhqt.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtivaympkd.html

[U78] PHP：单元测试
来源：http://hz.zycfv.cn/gtfovbchij.html

composer require --dev phpunit/phpunit
来源：http://hz.yj20258.top/gtimaikjcf.html

[U79] PHP：静态分析
来源：http://hz.zhixingplan.top/gthqkxvebp.html

composer require --dev phpstan/phpstan
来源：http://hz.shuidangran.top/gtkmnpfiyj.html

[U80] PHP：代码规范修复
来源：http://hz.xylfe.cn/gtfyncckit.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daxiang520.top/gtwyxnigxm.html

[U81] JS：初始化项目
来源：http://hz.meibo888.top/gtcxqfhgtq.html

npm init -y;  npm i express
来源：http://hz.yuxming.cn/gtqufbkiry.html

[U82] JS：package.json 脚本
来源：http://hz.hywenlv.cn/gtzftlalcm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cqqwz.cn/gtokqhdepp.html

[U83] JS：ES Module 导入导出
来源：http://hz.fengsongda.top/gtxxiinnpv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.redwolf501.top/gtnkleogvm.html

[U84] JS：CommonJS 写法
来源：http://hz.tian-w.cn/gtdlajrslw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cashguo.top/gtblgwdyti.html

[U85] JS：可选链
来源：http://hz.zhoulong.xyz/gtxlqqqhnf.html

a?.b?.c
来源：http://hz.ybcxt.top/gtoshmqjyh.html

[U86] JS：空值合并
来源：http://hz.cqqwz.cn/gtfiyesold.html

a ?? b
来源：http://hz.jinqigfzy.top/gtmknvkofl.html

[U87] JS：解构默认值
来源：http://hz.c1oappe.top/gtbdhltrlw.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhiwuduotai.top/gtsfrjikey.html

[U88] JS：对象展开合并
来源：http://hz.gzhubu.top/gtfojepxmz.html

{ ...a, ...b }
来源：http://hz.xuetiantiany.cn/gtiwoyznrq.html

[U89] JS：数组去重
来源：http://hz.yongpay.top/gtdakygjys.html

[...new Set(arr)]
来源：http://hz.0kj1m.cn/gtnbagwlwk.html

[U90] JS：数字数组排序
来源：http://hz.yj20258.top/gtvajtfwpx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtpuodymik.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtlupyszxy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nanxuanxn.top/gtqxojchnj.html

[U92] JS：深拷贝
来源：http://hz.redwolf501.top/gtpvpxtmhz.html

structuredClone(obj)
来源：http://hz.redwolf501.top/gtgflecamt.html

[U93] JS：模板字符串
来源：http://hz.hnqzz.top/gtgipsumxq.html

`共 ${n} 条`
来源：http://hz.xingfuxueyuan.xyz/gtxalvnsvn.html

[U94] JS：箭头函数
来源：http://hz.jinghuilouyu.cn/gtflaqtkhn.html

const double = x => x * 2;
来源：http://hz.kuanghao11.cn/gtqcivlvhr.html

[U95] JS：Promise 包装
来源：http://hz.xuetiantiany.cn/gttrhlhpyz.html

new Promise((resolve, reject) => {})
来源：http://hz.cqqwz.cn/gtewqvbsuk.html

[U96] JS：async/await 与异常
来源：http://hz.zhongyouzk.top/gtqmjtgvgy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtmztzoexq.html

[U97] JS：并发请求
来源：http://hz.birdmap.top/gtpcykwbly.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtdnyiyezq.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangshuangyany.cn/gtlzeeokfg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ywan-chungtsiang.top/gtisdhoerl.html

[U99] JS：事件监听
来源：http://hz.jinghuilouyu.cn/gthtqorjvz.html

el.addEventListener("click", e => {})
来源：http://hz.nwbrower.top/gtiootftge.html

[U100] JS：DOM 查询
来源：http://hz.yvedp.cn/gtwbvynfgr.html

document.querySelector(".item")
来源：http://hz.cucudq.cn/gtgzljmfhy.html

[U101] JS：classList 操作
来源：http://hz.ybcxt.top/gtyscmdatn.html

el.classList.toggle("active")
来源：http://hz.zhixingplan.top/gtjkyrcgsg.html

[U102] JS：本地存储
来源：http://hz.zhongyouzk.top/gthrqnjyli.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.fengsongda.top/gtdvxgcujr.html

[U103] JS：定时器
来源：http://hz.guannengcc.top/gtpmysohmx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhoulong.xyz/gtcjoxclbe.html

[U104] JS：防抖
来源：http://hz.gogol.net.cn/gtkfpgjwrn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtkkskzcfi.html

[U105] JS：节流
来源：http://hz.gzhubu.top/gtwzoinbnp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhongyouzk.top/gtelldpvyg.html

[U106] JS：日期格式化
来源：http://hz.ehwqpu.com/gtczntheim.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtlikznkxx.html

[U107] JS：数字千分位
来源：http://hz.c1oappe.top/gtndeeusrm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.0kj1m.cn/gtslamkorf.html

[U108] JS：随机整数
来源：http://hz.yj20258.top/gthwwgflgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yuanzhike.top/gthwwgkjcd.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtvgtvphgj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtuzuupnge.html

[U110] JS：数组分块
来源：http://hz.daxiang520.top/gtdlqlhspw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gtkdklfvfu.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtxgjhyzex.html

new Map(Object.entries(obj))
来源：http://hz.havefunace.top/gtukpunbyx.html

[U112] JS：字符串补位
来源：http://hz.yonumen.top/gtvloqompa.html

"7".padStart(3, "0")
来源：http://hz.yongpay.top/gtxpfivzej.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gtuuzxeanm.html

s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtippbtcka.html

[U114] JS：JSON 深比较
来源：http://hz.chenzaomai.com/gtgvqcvnsw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtjmakxvmn.html

[U115] JS：生成 UUID
来源：http://hz.andypj.xyz/gtqesjnawm.html

crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtfyumdfwm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.meibo888.top/gtvyvcjeeg.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sufxvd.cn/gtgdicdjlo.html

[U117] JS：单元测试
来源：http://hz.xziqi.cn/gtejehoewp.html

npm i -D vitest;  npx vitest
来源：http://hz.jinqigfzy.top/gtwwzfdwzd.html

[U118] JS：开发服务器
来源：http://hz.nwbrower.top/gtqdzjlzfw.html

npm i -D vite;  npx vite
来源：http://hz.jqgufenzy.top/gtcwqxvcvt.html

[U119] JS：生产构建
来源：http://hz.hammf.cn/gtyfcncdmx.html

npx vite build
来源：http://hz.ybcxt.top/gtranvujnp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jlsjyb.cn/gtbvqjmhwr.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangkeji.top/gtmrggyhso.html

================================================================================
来源：http://hz.bjfxy.top/gtxkloorkv.html

统计汇总
来源：http://hz.jqgufenzy.top/gtspvxfmcm.html

================================================================================
来源：http://hz.ybcxt.top/gtpefrjlth.html

按语言统计（条）：
来源：http://hz.yanxiufei.cn/gtlpjrxowl.html

Python ......... 252
来源：http://hz.jqgfzy.top/gteidpatfh.html

PHP ............ 252
来源：http://hz.ivvv.top/gtltnygxwo.html

JavaScript ..... 252
来源：http://hz.jinqigufen.top/gtdsztjnnm.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtsgtfyszo.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtgqyqmqlz.html

Go ............. 212
来源：http://hz.andypj.xyz/gtelfacjvy.html

Ruby ........... 212
来源：http://hz.jianghu66.top/gttwnstjim.html

C# ............. 212
来源：http://hz.gzhubu.top/gtkarpglen.html

C .............. 30
来源：http://hz.hnxiangtu.top/gtesizsgoz.html

C++ ............ 30
来源：http://hz.hywenlv.cn/gtsnueeikb.html

SQL ............ 90
来源：http://hz.smart0.xyz/gtyeiacofu.html

Bash ........... 80
来源：http://hz.jinyuanbaomall.cn/gtxzaucylf.html

Kotlin ......... 15
来源：http://hz.aibaodan.cn/gtgdixftul.html

Swift .......... 15
来源：http://hz.xuetiantiany.cn/gttbqyqlxc.html

Lua ............ 10
来源：http://hz.zhengqikj.top/gtvvzpnlaj.html

Perl ........... 10
来源：http://hz.birdmap.top/gtaxvduxcl.html

Scala .......... 10
来源：http://hz.hammf.cn/gtgpvioioc.html

------------------------------------
来源：http://hz.nanxinkj.top/gtgxajmsll.html

合计 ........... 2106 条
来源：http://hz.9152youxi.cn/gtktwtjbey.html

按章节统计：
来源：http://hz.hongshengwenyu.top/gtjfwtrqsz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtsfvwhyxx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtecvacgcz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtlrxjfjve.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cashguo.top/gtydganmpx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtlmbbhghi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtudyqezoi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ppjwa.cn/gteyorukre.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtzfwgxcrd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtuiriqgxe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gogol.net.cn/gtlomdqtub.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtcojayesn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gttcobqoeb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtujjxannk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ybcxt.top/gtrkecnhpb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.havefunace.top/gtalogliho.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtdtutfcef.html

Q SQL 专题                              90
来源：http://hz.nwbrower.top/gtwtntqvcj.html

R Bash 专题                             80
来源：http://hz.ywan-chungtsiang.top/gtchmiubhr.html

S C / C++ 专题                          60
来源：http://hz.hywenlv.cn/gtnjxdwcic.html

T 其他语言补充                          60
来源：http://hz.yj20258888.top/gtxmhtvlbr.html

U 高频实用片段                         120
来源：http://hz.wangshuangyany.cn/gtmhpctjds.html

------------------------------------
来源：http://hz.jyoumei.cn/gthcyonitl.html

合计                                  2106 条
来源：http://hz.nanxuanxn.top/gtpanumugk.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtclcbtprp.html

使用提醒
来源：http://hz.chenjidiqi.icu/gtpzxmuwrj.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtnkkapivc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.feifeiyinyue.top/gtibftvgvy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhaomingkeji.xyz/gtplpqkivi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.52xcode.cn/gtagkjnabm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.snrcjt.cn/gtihhjlpfd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ybcxt.top/gtlvcdaukg.html

—— 文件结束 ——
来源：http://hz.daria6918.cn/gttlpqdqzg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzrjntfae.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tianlin.xyz/gtrckuyvdo.html

Common Programming Examples Cheat Book
来源：http://hz.hammf.cn/gtglgivlhf.html

================================================================================
来源：http://hz.fzhhl.top/gtdkwaibqr.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtwvyzizmv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhaomingkeji.xyz/gtbtrfbcwv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.meibo888.top/gtwjvhfwxx.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gtcvwlorbn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.sufxvd.cn/gtafjiqsmj.html

【使用说明】
来源：http://hz.jinyuanbaomall.cn/gtixaixpfd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinghuilouyu.cn/gtgoptawuw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yanxiufei.cn/gtzifkanmi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.wangshuangyany.cn/gtscehvinx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yvedp.cn/gtyzfekvcc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigfzy.top/gtghnppdjg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.sysykeji.top/gtuydepoop.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zdqjudy.top/gtprnftmxj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.cqqwz.cn/gtqmjgxvgo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhiwuduotai.top/gtchpkwrxm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jyoumei.cn/gtbqdbvrvp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zycfv.cn/gtbwqmyzbn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.pycfn.com/gtdzybcmgf.html

【文件统计】
来源：http://hz.ivvv.top/gthgcyognu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cqqwz.cn/gthainjaun.html

--------------------------------------------------------------------------------
来源：http://hz.dashuyun.cn/gtseoytypp.html

目  录
来源：http://hz.yonumen.top/gtnctsdqap.html

--------------------------------------------------------------------------------
来源：http://hz.zhengqikj.top/gtsctmclil.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtynpqiqub.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hammf.cn/gtwwbzuujs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtgcqvunbj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtjsmfsvzw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zycfv.cn/gtvgefrytl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhengqikj.top/gtflewwkjp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.chenjidiqi.icu/gttmqlzpzz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sysykeji.top/gtjdncvzty.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtvsmltlvh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gtewtzvspz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtmasjnuip.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtohcgsutu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtyqnpgezz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.vqdsnc.cn/gthwrvdifb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.pengpengdd.cyou/gthaecnwto.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nanxuanxn.top/gtnzgwwfki.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sxryk.cn/gtrroffpvy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xuetiantiany.cn/gtahpluejh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgufenzy.top/gtpxrwqiwg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtgtjkizvt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtgvjjimvn.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkmanpzpk.html

A. 基础语法与类型
来源：http://hz.yonumen.top/gtsaloupql.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsamaaxcl.html

[A01] Hello World
来源：http://hz.yj20258.top/gtounrczzf.html

Py:   print("Hello, World!")
来源：http://hz.meibo888.top/gtwaxmsxcl.html

PHP:  echo "Hello, World!";
来源：http://hz.cheryme.top/gtwlvndalm.html

JS:   console.log("Hello, World!");
来源：http://hz.gaohongyu789.top/gtrchdztmn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sufxvd.cn/gtnkrahvyt.html

Java: System.out.println("Hello, World!");
来源：http://hz.yangfankeji.com/gtdeqmlcig.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.dashuyun.cn/gtnpkctavt.html

Ruby: puts "Hello, World!"
来源：http://hz.chenzaomai.com/gtqxumaklv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zdqjudy.top/gtwfrkrmdr.html

[A02] 变量声明与赋值
来源：http://hz.hysaishi.cn/gtsnazghgk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.fzhhl.top/gtgyengemd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hfpthk.cn/gtdqdgpfez.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuanzx.com/gtiqecvtug.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zycfv.cn/gtdhkkbkuc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sxryk.cn/gtxitaqaqa.html

Go:   name := "Alex"; age := 20
来源：http://hz.jlsjyb.cn/gtnwjhmhqh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gtrhgewwoi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhongyouzk.top/gtrhhenhcn.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtyzvyhtse.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinqigfzy.top/gtjzofmsqx.html

PHP:  const PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtfnkabckp.html

JS:   const PI = 3.14159;
来源：http://hz.xuanzx.com/gtdwhvbsnm.html

TS:   const PI: number = 3.14159;
来源：http://hz.xylfe.cn/gtgdvcddpu.html

Java: static final double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtwvwogolk.html

Go:   const PI = 3.14159
来源：http://hz.dashuyun.cn/gttnaenmks.html

Ruby: PI = 3.14159
来源：http://hz.ydjk.org.cn/gtrvygvjpn.html

C#:   const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtwxkcqfpb.html

[A04] 判断变量类型
来源：http://hz.sxryk.cn/gtsnggjupi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yvedp.cn/gtkqplhorz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jqgufenzy.top/gtsieahzvm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yuanzhike.top/gtflbpodrw.html

TS:   typeof x; x instanceof Date
来源：http://hz.xinyue.icu/gtjpblpyrq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yonumen.top/gtyqxhuxfk.html


<!-- 参考信息 -->