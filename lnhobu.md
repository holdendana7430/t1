代发 wailian999

[U37] Py：读写 Excel
来源：http://hz.hywenlv.cn/gtjoppazmh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuxming.cn/gtfzgnkvsr.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gtxsxxmegs.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtchjitzzw.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtpnwdvpxi.html

sys.stdout.isatty()
来源：http://hz.hnqzz.top/gtfthgmvhw.html

[U40] Py：打印到标准错误
来源：http://hz.chenzaomai.com/gtfcuijied.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtmvfbjsxm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gtpnqhocpy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nwbrower.top/gtrwbcpben.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinyuanbaomall.cn/gtvuecdaex.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sweek.top/gtmlqzhqgs.html

[U43] PHP：声明命名空间
来源：http://hz.hammf.cn/gtvlgqugrk.html

namespace App\Http;
来源：http://hz.zhaomingkeji.xyz/gtzbsaaske.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtryhuhmem.html

declare(strict_types=1);
来源：http://hz.hnxiangtu.top/gtgwjrpjvi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yanxiufei.cn/gtftktzabr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtqyswwtyn.html

[U46] PHP：可空类型
来源：http://hz.jinyuanbaomall.cn/gtgjcahujr.html

?string $name = null
来源：http://hz.zhixingplan.top/gtiokztuld.html

[U47] PHP：联合类型
来源：http://hz.daxiang520.top/gtvtetzksv.html

int|string $id
来源：http://hz.ivvv.top/gtalndbbew.html

[U48] PHP：纯枚举
来源：http://hz.jinyuanbaomall.cn/gtefyhxjss.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shuidangran.top/gtvjobvbua.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gthrszjesg.html

public readonly string $name
来源：http://hz.zhixingplan.top/gtzevtamvm.html

[U50] PHP：构造器属性提升
来源：http://hz.chenlongwang.top/gtmkbxmvve.html

public function __construct(private int $id) {}
来源：http://hz.wangshuangyany.cn/gtywcvcjhu.html

[U51] PHP：数组解构
来源：http://hz.sweek.top/gtheornlse.html

[$a, $b] = $arr;
来源：http://hz.yangfankeji.com/gtzjjhrvrz.html

[U52] PHP：箭头函数
来源：http://hz.yongpay.top/gtmooivpwx.html

$double = fn($x) => $x * 2;
来源：http://hz.fengsongda.top/gtwnojwakb.html

[U53] PHP：空合并运算符
来源：http://hz.yongpay.top/gtxnbhghze.html

$v = $a ?? $b ?? "default";
来源：http://hz.zycfv.cn/gtnopwphwd.html

[U54] PHP：空安全调用
来源：http://hz.sweek.top/gtgysmxwwv.html

$obj?->method()
来源：http://hz.hfpthk.cn/gtwnzjepaa.html

[U55] PHP：match 表达式
来源：http://hz.yj20258888.top/gtxxiqtoxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aizwys.cn/gtopqodgvz.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtlbmdxcbo.html

f(a: 1, b: 2)
来源：http://hz.ivvv.top/gtpogkfqgs.html

[U57] PHP：字符串插值
来源：http://hz.ehwqpu.com/gtpacxkuos.html

"值: {$a}"
来源：http://hz.snrcjt.cn/gtdblpxszj.html

[U58] PHP：数组三件套
来源：http://hz.dashuyun.cn/gtckelwywm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yonumen.top/gteerljfmo.html

[U59] PHP：自定义排序
来源：http://hz.cashguo.top/gtkoizewrp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtetlkpeto.html

[U60] PHP：JSON 编解码
来源：http://hz.haohaochexian.top/gtsexqimsy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fzhhl.top/gtcutzmqzf.html

[U61] PHP：正则
来源：http://hz.jyoumei.cn/gtagxgmobn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtkbtokuag.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtvrlfecug.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gtthumbadf.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gtoioyhjuu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.haohaochexian.top/gtytvtvmrq.html

[U64] PHP：目录遍历
来源：http://hz.haohaochexian.top/gtbkmkbvra.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gotoacloud.top/gtgoivihmr.html

[U65] PHP：会话
来源：http://hz.ivvv.top/gtqnmicped.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.haohaochexian.top/gtnaffyoxa.html

[U66] PHP：设置 Cookie
来源：http://hz.gaohongyu789.top/gtpzbjianw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj202588.top/gthlyeqrpf.html

[U67] PHP：处理文件上传
来源：http://hz.jinqigfzy.top/gtbkkwpvqn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtmpvidkzj.html

[U68] PHP：PDO 连接
来源：http://hz.dianchejie.cn/gtionetdhe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.iojbl.cn/gthtguegmo.html

[U69] PHP：PDO 预处理
来源：http://hz.hysaishi.cn/gtmpuxmdjj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xinyue.icu/gtmnmpvtyj.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtaupcwudr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuanzx.com/gtxkwilldo.html

[U71] PHP：抛出异常
来源：http://hz.yj20258888.top/gtpuqirckw.html

throw new RuntimeException("失败", 500);
来源：http://hz.gaohongyu789.top/gtkjczimcf.html

[U72] PHP：写错误日志
来源：http://hz.mhx1999.top/gtpmzaflto.html

error_log("失败: " . $e->getMessage());
来源：http://hz.sufxvd.cn/gtkohydwqs.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinyuanbaomall.cn/gtikqhjfyi.html

parse_ini_file("config.ini", true)
来源：http://hz.snrcjt.cn/gtpkbqyrky.html

[U74] PHP：读取环境变量
来源：http://hz.tianlin.xyz/gtfoxmwhfm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hammf.cn/gtnckwfshp.html

[U75] PHP：依赖注入
来源：http://hz.pengpengdd.cyou/gtgvmwersp.html

composer require psr/container
来源：http://hz.iojbl.cn/gtqsjricqd.html

[U76] PHP：简单路由
来源：http://hz.jqgufenzy.top/gtqvharvbd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.feifeiyinyue.top/gtoeggkktn.html

[U77] PHP：模板渲染
来源：http://hz.xuetiantiany.cn/gtssoojolj.html

composer require twig/twig
来源：http://hz.guowangkeji.top/gtumhabyog.html

[U78] PHP：单元测试
来源：http://hz.fengsongda.top/gtmrjublom.html

composer require --dev phpunit/phpunit
来源：http://hz.hongshengwenyu.top/gtvvcaqjpz.html

[U79] PHP：静态分析
来源：http://hz.yuxming.cn/gtynzmqzgv.html

composer require --dev phpstan/phpstan
来源：http://hz.aizwys.cn/gtmvuvyvkv.html

[U80] PHP：代码规范修复
来源：http://hz.hammf.cn/gttukzxzbl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.0kj1m.cn/gtbdgheios.html

[U81] JS：初始化项目
来源：http://hz.tianlin.xyz/gtrmtepppp.html

npm init -y;  npm i express
来源：http://hz.jyoumei.cn/gthnrapzst.html

[U82] JS：package.json 脚本
来源：http://hz.jinqigufen.top/gthknrocig.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxuanxn.top/gtmqsetqoo.html

[U83] JS：ES Module 导入导出
来源：http://hz.daxiang520.top/gtejkzsbgl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.birdmap.top/gtlbfylzyr.html

[U84] JS：CommonJS 写法
来源：http://hz.ehwqpu.com/gtojvkkkxb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yongpay.top/gtrifvkbie.html

[U85] JS：可选链
来源：http://hz.zhongyouzk.top/gtkzpyqrbs.html

a?.b?.c
来源：http://hz.aizwys.cn/gtxjvhyitd.html

[U86] JS：空值合并
来源：http://hz.jyoumei.cn/gtsvsnzvbe.html

a ?? b
来源：http://hz.jqgfzy.top/gthhpuqnhc.html

[U87] JS：解构默认值
来源：http://hz.wangshuangyany.cn/gtggckapkp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.daxiang520.top/gtikqhzwdf.html

[U88] JS：对象展开合并
来源：http://hz.sufxvd.cn/gtzhuhfvjd.html

{ ...a, ...b }
来源：http://hz.nanxinkj.top/gttoqubavo.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gtwnsrnsra.html

[...new Set(arr)]
来源：http://hz.yj20258888.top/gtszwgpvvt.html

[U90] JS：数字数组排序
来源：http://hz.yangfankeji.com/gtwofmgdvi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gttpenpmys.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangtech.top/gtcddyfcrd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xuanzx.com/gtfxvrjcsi.html

[U92] JS：深拷贝
来源：http://hz.zhixingplan.top/gthnpecgfe.html

structuredClone(obj)
来源：http://hz.hammf.cn/gtmmsrxgqf.html

[U93] JS：模板字符串
来源：http://hz.tianlin.xyz/gtebpfjymg.html

`共 ${n} 条`
来源：http://hz.hywenlv.cn/gtelmkqoel.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtfsdbscna.html

const double = x => x * 2;
来源：http://hz.aibaodan.cn/gtlfxpvbmp.html

[U95] JS：Promise 包装
来源：http://hz.xingfuxueyuan.xyz/gtqmdhlqvu.html

new Promise((resolve, reject) => {})
来源：http://hz.zhixingplan.top/gtuothoetm.html

[U96] JS：async/await 与异常
来源：http://hz.zycfv.cn/gtbkvnexxo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gteosxhneb.html

[U97] JS：并发请求
来源：http://hz.zhoulong.xyz/gtwvbnjyih.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtrjhzkarf.html

[U98] JS：fetch 带 JSON
来源：http://hz.fengsongda.top/gttkujrxcl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yonumen.top/gtpzbocmrb.html

[U99] JS：事件监听
来源：http://hz.redwolf501.top/gtkgwpywxy.html

el.addEventListener("click", e => {})
来源：http://hz.fengsongda.top/gtjkiiynod.html

[U100] JS：DOM 查询
来源：http://hz.kuanghao11.cn/gtapfmurjz.html

document.querySelector(".item")
来源：http://hz.kuanghao11.cn/gthokssrpm.html

[U101] JS：classList 操作
来源：http://hz.wangdashe.top/gtdixvdcdt.html

el.classList.toggle("active")
来源：http://hz.shuidangran.top/gtjoxkghcj.html

[U102] JS：本地存储
来源：http://hz.yuxming.cn/gtbpftozfq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tian-w.cn/gtisneyaoo.html

[U103] JS：定时器
来源：http://hz.52xcode.cn/gtilnveuie.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.birdmap.top/gtqofpahhq.html

[U104] JS：防抖
来源：http://hz.xuetiantiany.cn/gthhvbbfjq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.birdmap.top/gtyqajmcew.html

[U105] JS：节流
来源：http://hz.yj20258.top/gtnpspzsca.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtxadxjbtf.html

[U106] JS：日期格式化
来源：http://hz.ywan-chungtsiang.top/gtipagvpdq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxinkj.top/gtjyhgikhf.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtvwvdglyy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aibaodan.cn/gtrkurkmdt.html

[U108] JS：随机整数
来源：http://hz.aibaodan.cn/gtlxhjwfpn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tanke756.top/gtbenxowiq.html

[U109] JS：数组分组
来源：http://hz.fengsongda.top/gtzdqbudbi.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gtswljolyp.html

[U110] JS：数组分块
来源：http://hz.cashguo.top/gtskwjfhgw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hysaishi.cn/gtijpxrhav.html

[U111] JS：对象转 Map
来源：http://hz.svipenyu.cn/gtgmmuwbkg.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gtbxxigwjk.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtpdmotooi.html

"7".padStart(3, "0")
来源：http://hz.yonumen.top/gtdhydogox.html

[U113] JS：正则替换全部
来源：http://hz.yj20258.top/gtraqmeepq.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtdvhjtpak.html

[U114] JS：JSON 深比较
来源：http://hz.zhongyouzk.top/gtdtimlbjj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtyvntbjdp.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gtslypscya.html

crypto.randomUUID()
来源：http://hz.birdmap.top/gtwfqunsgg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.mhx1999.top/gtkqsbssmm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gogol.net.cn/gtbmveivzk.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtvywemcsp.html

npm i -D vitest;  npx vitest
来源：http://hz.iojbl.cn/gtctjipcoi.html

[U118] JS：开发服务器
来源：http://hz.jyoumei.cn/gtfslclnap.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gtktpjdaka.html

[U119] JS：生产构建
来源：http://hz.svipenyu.cn/gtfyctxmbg.html

npx vite build
来源：http://hz.pengpengdd.cyou/gtumeztjby.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.c1oappe.top/gtcyjaehlw.html

import.meta.env.VITE_API_URL
来源：http://hz.hammf.cn/gtufozpknv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrvqnvsps.html

统计汇总
来源：http://hz.mhx1999.top/gtaiaiyyqk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxbltomby.html

按语言统计（条）：
来源：http://hz.shzxlz.cn/gtgcpkruuq.html

Python ......... 252
来源：http://hz.ydzc1.top/gtdgunxuhh.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gtfxnphvwg.html

JavaScript ..... 252
来源：http://hz.shanyushiyangtech.top/gtqmndalgn.html

TypeScript ..... 212
来源：http://hz.chenlongwang.top/gtlqyejcmb.html

Java ........... 212
来源：http://hz.nanxuanxn.top/gtzcmorcwh.html

Go ............. 212
来源：http://hz.smart0.xyz/gtwemmambx.html

Ruby ........... 212
来源：http://hz.yangfankeji.com/gtqgspioxj.html

C# ............. 212
来源：http://hz.jqgfzy.top/gtwjoxgdma.html

C .............. 30
来源：http://hz.cashguo.top/gtjcqedgjj.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtuwohoicl.html

SQL ............ 90
来源：http://hz.shzxlz.cn/gtadqlcfcv.html

Bash ........... 80
来源：http://hz.0kj1m.cn/gtgevuxmll.html

Kotlin ......... 15
来源：http://hz.sweek.top/gtmsaldhbn.html

Swift .......... 15
来源：http://hz.nanxinkj.top/gtrvticiis.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtipetavez.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gtbvnnxlod.html

Scala .......... 10
来源：http://hz.nanxinkj.top/gthqtzbwii.html

------------------------------------
来源：http://hz.zhengqikj.top/gtqoxkqqqg.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gthkdtyguh.html

按章节统计：
来源：http://hz.jiagoushi.top/gtcfoqnddl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangdashe.top/gtjflbyuhb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gttaylodgl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtzmfohnpl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtyoafmboi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.bjfxy.top/gtxexkdotj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtsllifibs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.xziqi.cn/gtkorymwir.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258.top/gtyxciulfh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtjebszxrf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.svipenyu.cn/gtykpkinst.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtskgpdnzr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtiyfcvjgx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtibjoajpx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gtuamdrknp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.havefunace.top/gtkibzanar.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtwxvymtls.html

Q SQL 专题                              90
来源：http://hz.mhx1999.top/gtguwhfzcd.html

R Bash 专题                             80
来源：http://hz.yuanzhike.top/gtjpixzljm.html

S C / C++ 专题                          60
来源：http://hz.hnqzz.top/gtuzhgzuyx.html

T 其他语言补充                          60
来源：http://hz.zhijiandao.cn/gtegspwess.html

U 高频实用片段                         120
来源：http://hz.jqgfzy.top/gtmuxspvmb.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtttgldunr.html

合计                                  2106 条
来源：http://hz.nwbrower.top/gtpuxowmfx.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gtpalnxmxs.html

使用提醒
来源：http://hz.nanxinkj.top/gtzqzojmgs.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gteqeogpuh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydzc1.top/gtrpvlxdrv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.andypj.xyz/gtsygnenmx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jinyuanbaomall.cn/gtzmqxlfmk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hongshengwenyu.top/gtzdiqbrny.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.9152youxi.cn/gteoaikbeb.html

—— 文件结束 ——
来源：http://hz.chenzaomai.com/gtsffcwdjf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtesjpruxh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinqigufen.top/gthcugbqtv.html

Common Programming Examples Cheat Book
来源：http://hz.xuanzx.com/gtebukjiad.html

================================================================================
来源：http://hz.ivvv.top/gtomwfuiom.html

【收录内容】
来源：http://hz.hnxiangtu.top/gtwquyfjao.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.guannengcc.top/gtiahinsdo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xylfe.cn/gtscdvhple.html

SQL · Bash · C · C++
来源：http://hz.yanxiufei.cn/gteunntuyf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.aizwys.cn/gtmofoonam.html

【使用说明】
来源：http://hz.bjfxy.top/gtylazfqam.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gotoacloud.top/gtfsxwpxyn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.tian-w.cn/gtcfaqvszb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jinghuilouyu.cn/gtnwgdmhhe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenlongwang.top/gtvwhwjzsw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.0kj1m.cn/gtjhbnlvuv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gtzwottpap.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtugejmrpf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.andypj.xyz/gtgsxymhxs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.pycfn.com/gtiehapfjm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shanyushiyangkeji.top/gtljncznjk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.52xcode.cn/gtgxbdurhb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ydzc1.top/gtmtaxltri.html

【文件统计】
来源：http://hz.daria6918.cn/gtiwlgwfvt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gtzldasbzv.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtrrvkjxhk.html

目  录
来源：http://hz.snrcjt.cn/gtpccdrcwq.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtvnrgrvwo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hfpthk.cn/gtsrcwyfzb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtveksfqkh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.meibo888.top/gttoomommr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shanyushiyangkeji.top/gtxwepcstn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xuetiantiany.cn/gtmbtavhvc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ivvv.top/gtqsictupy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtgjikbumc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtphxuaasv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtmvblzapf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jqgufenzy.top/gtfkyrfnqf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtcnawcrjt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gttoysxbdq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtndkuoqfb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.guowangkeji.top/gtbuttfpmq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jyoumei.cn/gtcprmqzsd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtvzjibroh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.quarkkingdee.top/gtbajlodfr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xuetiantiany.cn/gtxrfgmpof.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hfpthk.cn/gthlkbueme.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtbrksswin.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtgkhggnop.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttdtqredb.html

A. 基础语法与类型
来源：http://hz.shangyingyoupin.top/gtigzhtxcx.html

================================================================================
来源：http://hz.jianghu66.top/gtxkrwxxbb.html

[A01] Hello World
来源：http://hz.nwbrower.top/gtmwmgjcwv.html

Py:   print("Hello, World!")
来源：http://hz.sweek.top/gtyqourrpf.html

PHP:  echo "Hello, World!";
来源：http://hz.hammf.cn/gtxgioyfkt.html

JS:   console.log("Hello, World!");
来源：http://hz.xylfe.cn/gtnkhvhuyy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.hysaishi.cn/gtupltggsk.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtwypcyodb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhengqikj.top/gtcmkbpjba.html

Ruby: puts "Hello, World!"
来源：http://hz.jlsjyb.cn/gtnhxgdszn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhiwuduotai.top/gtwaytrabz.html

[A02] 变量声明与赋值
来源：http://hz.hnxiangtu.top/gthhtreocy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.quarkkingdee.top/gthuaiugoz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinghuilouyu.cn/gtjkuxhhen.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhijiandao.cn/gtfpadqxos.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yanxiufei.cn/gtpuylhygx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtwrskessr.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenlongwang.top/gtrthcpwhs.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guannengcc.top/gtwzrlgsgs.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nanxinkj.top/gtispznabg.html

[A03] 常量定义
来源：http://hz.haohaochexian.top/gtrumlwgxv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.xinyue.icu/gtmjcqdczy.html

PHP:  const PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtzokcihgi.html

JS:   const PI = 3.14159;
来源：http://hz.sweek.top/gtolscqxig.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtfsroaygb.html

Java: static final double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtiktiieur.html

Go:   const PI = 3.14159
来源：http://hz.zhaomingkeji.xyz/gtyrcilkvt.html


<!-- 参考信息 -->