代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinyuanbaomall.cn/gtsufbekus.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shuidangran.top/gtpzqufgjq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.tian-w.cn/gtyodpnrcn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhiwuduotai.top/gthczntoyk.html

[U43] PHP：声明命名空间
来源：http://hz.jlsjyb.cn/gtxtneoqov.html

namespace App\Http;
来源：http://hz.jinqigufen.top/gtmjqbxikl.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtuhtgzlrm.html

declare(strict_types=1);
来源：http://hz.fzhhl.top/gtfitqtoaj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gtoxeaihap.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtbbzuebnd.html

[U46] PHP：可空类型
来源：http://hz.ehwqpu.com/gtzaorwbeg.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtlrjtdsan.html

[U47] PHP：联合类型
来源：http://hz.yj20258.top/gthdazpmka.html

int|string $id
来源：http://hz.shanyushiyangtech.top/gtqsuzeaeo.html

[U48] PHP：纯枚举
来源：http://hz.jqgfzy.top/gtldljheds.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhoulong.xyz/gtybdbvznh.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gttvohidzt.html

public readonly string $name
来源：http://hz.iojbl.cn/gtvyimhkag.html

[U50] PHP：构造器属性提升
来源：http://hz.pycfn.com/gtveodoprt.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtnwgdjvbp.html

[U51] PHP：数组解构
来源：http://hz.tanke756.top/gtamrkehsr.html

[$a, $b] = $arr;
来源：http://hz.0kj1m.cn/gtujcyscap.html

[U52] PHP：箭头函数
来源：http://hz.smart0.xyz/gtjfowbbyh.html

$double = fn($x) => $x * 2;
来源：http://hz.yuxming.cn/gtaclrfjso.html

[U53] PHP：空合并运算符
来源：http://hz.chenzaomai.com/gtoldmsdim.html

$v = $a ?? $b ?? "default";
来源：http://hz.gogol.net.cn/gtcofzziek.html

[U54] PHP：空安全调用
来源：http://hz.zycfv.cn/gtynsspkcd.html

$obj?->method()
来源：http://hz.vqdsnc.cn/gthplsttjv.html

[U55] PHP：match 表达式
来源：http://hz.xziqi.cn/gtsknxpbvz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cheryme.top/gtxhnqiuhq.html

[U56] PHP：命名参数
来源：http://hz.sxryk.cn/gtpzkcmqjm.html

f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtbgshzmrr.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtpbvaatsx.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtvsihruoq.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gthrzfheya.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hysaishi.cn/gtwcbwkjgi.html

[U59] PHP：自定义排序
来源：http://hz.hnqzz.top/gtvscfeyqn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtpetynvka.html

[U60] PHP：JSON 编解码
来源：http://hz.xingfuxueyuan.xyz/gtjnllvqwo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tian-w.cn/gtiaojadua.html

[U61] PHP：正则
来源：http://hz.dianchejie.cn/gtauopseha.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gtfufbswij.html

[U62] PHP：日期对象
来源：http://hz.shangyingyoupin.top/gtqkoibnux.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shzxlz.cn/gtxvjwsdkc.html

[U63] PHP：文件读写
来源：http://hz.jianghu66.top/gtbagnayrd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gtcsreomsb.html

[U64] PHP：目录遍历
来源：http://hz.gaohongyu789.top/gtswtzlzsi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jinyuanbaomall.cn/gtrthvwtwv.html

[U65] PHP：会话
来源：http://hz.shangyingyoupin.top/gtenrslrio.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aibaodan.cn/gtvjcjmtto.html

[U66] PHP：设置 Cookie
来源：http://hz.ybcxt.top/gtqgrvruxe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258888.top/gtmqsqsnzg.html

[U67] PHP：处理文件上传
来源：http://hz.c1oappe.top/gthyxprdpq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jianghu66.top/gteatrwaei.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gtlhgovkxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinghuilouyu.cn/gtwvpgqxra.html

[U69] PHP：PDO 预处理
来源：http://hz.jyoumei.cn/gtqcrbyimp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gtxbxkdtwc.html

[U70] PHP：PDO 事务
来源：http://hz.mhx1999.top/gtnxtndugo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinqigfzy.top/gtyzqugvyl.html

[U71] PHP：抛出异常
来源：http://hz.jinqigfzy.top/gtxajkoyaf.html

throw new RuntimeException("失败", 500);
来源：http://hz.gotoacloud.top/gtqmutwaoa.html

[U72] PHP：写错误日志
来源：http://hz.daxiang520.top/gtoecotbpo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gaohongyu789.top/gtnvuufwfl.html

[U73] PHP：读取 ini 配置
来源：http://hz.cucudq.cn/gtleknxywh.html

parse_ini_file("config.ini", true)
来源：http://hz.ehwqpu.com/gtjseaflbw.html

[U74] PHP：读取环境变量
来源：http://hz.tanke756.top/gtezcvpouo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhoulong.xyz/gtnbosflgz.html

[U75] PHP：依赖注入
来源：http://hz.hysaishi.cn/gtulehfzcv.html

composer require psr/container
来源：http://hz.dashuyun.cn/gtqftrzrym.html

[U76] PHP：简单路由
来源：http://hz.chenzaomai.com/gtckkqraav.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sxryk.cn/gtfquufuvn.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gtcixenkvr.html

composer require twig/twig
来源：http://hz.shanyushiyangkeji.top/gtqvvpghdg.html

[U78] PHP：单元测试
来源：http://hz.quarkkingdee.top/gtbnlfderr.html

composer require --dev phpunit/phpunit
来源：http://hz.nanxuanxn.top/gtgfzxggpc.html

[U79] PHP：静态分析
来源：http://hz.jinyuanbaomall.cn/gtfqlroigo.html

composer require --dev phpstan/phpstan
来源：http://hz.daria6918.cn/gtdpiuakxk.html

[U80] PHP：代码规范修复
来源：http://hz.xuetiantiany.cn/gttchylfyl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.wangdashe.top/gtxqtajbxz.html

[U81] JS：初始化项目
来源：http://hz.fzhhl.top/gtdcinaosf.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtqkekfgfz.html

[U82] JS：package.json 脚本
来源：http://hz.yueranfly.top/gtqfcvkroz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sweek.top/gthktanaow.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangshuangyany.cn/gtynjsszht.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xylfe.cn/gtsitogyjr.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gtmivevqhf.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gttxrfmber.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gtodkqsjgn.html

a?.b?.c
来源：http://hz.hfpthk.cn/gttgczaodj.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtmsstcrgd.html

a ?? b
来源：http://hz.dianchejie.cn/gtmlaelofk.html

[U87] JS：解构默认值
来源：http://hz.xuetiantiany.cn/gtczctoqeo.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhengqikj.top/gtrzipwqik.html

[U88] JS：对象展开合并
来源：http://hz.ydzc1.top/gtdxboboar.html

{ ...a, ...b }
来源：http://hz.chenlongwang.top/gtazkzrrhu.html

[U89] JS：数组去重
来源：http://hz.yueranfly.top/gtqsciaxhj.html

[...new Set(arr)]
来源：http://hz.jyoumei.cn/gtydjgnfxk.html

[U90] JS：数字数组排序
来源：http://hz.c1oappe.top/gtekaczuoy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtnstvtgao.html

[U91] JS：对象键值遍历
来源：http://hz.tianlin.xyz/gtnkewlmno.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hammf.cn/gtafvjtzir.html

[U92] JS：深拷贝
来源：http://hz.aizwys.cn/gtjvomamdo.html

structuredClone(obj)
来源：http://hz.gotoacloud.top/gtpildkdld.html

[U93] JS：模板字符串
来源：http://hz.jinyuanbaomall.cn/gtvbekfqqy.html

`共 ${n} 条`
来源：http://hz.redwolf501.top/gtzdvafmep.html

[U94] JS：箭头函数
来源：http://hz.52xcode.cn/gtrolccqwl.html

const double = x => x * 2;
来源：http://hz.jqgufenzy.top/gtyoamunrh.html

[U95] JS：Promise 包装
来源：http://hz.cdnleiting.top/gtetkrjsqf.html

new Promise((resolve, reject) => {})
来源：http://hz.sysykeji.top/gtotvgrmdl.html

[U96] JS：async/await 与异常
来源：http://hz.havefunace.top/gtvxzxficx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gttntsvsqg.html

[U97] JS：并发请求
来源：http://hz.jinghuilouyu.cn/gtafaumxer.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtdegpdngx.html

[U98] JS：fetch 带 JSON
来源：http://hz.birdmap.top/gtxfrtaeuq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj202588.top/gtricwexxo.html

[U99] JS：事件监听
来源：http://hz.meibo888.top/gtwjgpoizo.html

el.addEventListener("click", e => {})
来源：http://hz.yuxming.cn/gtfewhqrzo.html

[U100] JS：DOM 查询
来源：http://hz.mhx1999.top/gtucbwyzkp.html

document.querySelector(".item")
来源：http://hz.zdqjudy.top/gtasmxjtva.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtfvfvntbv.html

el.classList.toggle("active")
来源：http://hz.zhongyouzk.top/gtlnhtroox.html

[U102] JS：本地存储
来源：http://hz.sxryk.cn/gtzgpmpsso.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sufxvd.cn/gtztaturjb.html

[U103] JS：定时器
来源：http://hz.0kj1m.cn/gtwujrlkyt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.iojbl.cn/gtsnrcmdgy.html

[U104] JS：防抖
来源：http://hz.ppjwa.cn/gtcyczepsh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtwomuziap.html

[U105] JS：节流
来源：http://hz.zhaomingkeji.xyz/gtzfphvedk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xuanzx.com/gtoebrgdpc.html

[U106] JS：日期格式化
来源：http://hz.9152youxi.cn/gtpmcfkfvp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj202588.top/gtrdwsbvcg.html

[U107] JS：数字千分位
来源：http://hz.hammf.cn/gtehbttabo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtzkbjuibr.html

[U108] JS：随机整数
来源：http://hz.zhaomingkeji.xyz/gtkcajxqhz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtuhgmcuxt.html

[U109] JS：数组分组
来源：http://hz.bjfxy.top/gtswxrgscp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtvmwvjxnd.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gtdlsbqhhp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gtcqjkvpcv.html

[U111] JS：对象转 Map
来源：http://hz.xziqi.cn/gtsqgvojme.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtemyixjsy.html

[U112] JS：字符串补位
来源：http://hz.jianghu66.top/gtoiqhcmyy.html

"7".padStart(3, "0")
来源：http://hz.ivvv.top/gtncwifowf.html

[U113] JS：正则替换全部
来源：http://hz.cqqwz.cn/gtcsuliodx.html

s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtjphigoci.html

[U114] JS：JSON 深比较
来源：http://hz.cashguo.top/gtpqaqnsvi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cheryme.top/gtlgcsotsr.html

[U115] JS：生成 UUID
来源：http://hz.wangdashe.top/gtrrrjjohy.html

crypto.randomUUID()
来源：http://hz.xziqi.cn/gtpztmbwwf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yongpay.top/gtqaerecmj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ivvv.top/gtfnnejoha.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gtzgmmnlwp.html

npm i -D vitest;  npx vitest
来源：http://hz.feifeiyinyue.top/gtrrlcivaj.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtcbgawawq.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtacphgsga.html

[U119] JS：生产构建
来源：http://hz.zhixingplan.top/gtqfvwwstk.html

npx vite build
来源：http://hz.yj20258888.top/gtfzaxpfwi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gtibovqipc.html

import.meta.env.VITE_API_URL
来源：http://hz.zhaomingkeji.xyz/gtkvlkftxp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtgepgnrjy.html

统计汇总
来源：http://hz.tian-w.cn/gtbzuiuexn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtmpnvxomz.html

按语言统计（条）：
来源：http://hz.gogol.net.cn/gtncbnmayr.html

Python ......... 252
来源：http://hz.fengsongda.top/gtvgmiymfz.html

PHP ............ 252
来源：http://hz.fengsongda.top/gtohsixaug.html

JavaScript ..... 252
来源：http://hz.kuanghao11.cn/gtmvgwpdxn.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtiinilwzf.html

Java ........... 212
来源：http://hz.andypj.xyz/gtuecpxsog.html

Go ............. 212
来源：http://hz.dashuyun.cn/gtdvwwisiv.html

Ruby ........... 212
来源：http://hz.feifeiyinyue.top/gtkumcjnrr.html

C# ............. 212
来源：http://hz.zhaomingkeji.xyz/gtdcjtrcmo.html

C .............. 30
来源：http://hz.sxryk.cn/gtuwzrslsp.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gtukswfbfv.html

SQL ............ 90
来源：http://hz.316326.xyz/gttmgethwi.html

Bash ........... 80
来源：http://hz.xylfe.cn/gtcypvfydn.html

Kotlin ......... 15
来源：http://hz.xziqi.cn/gtgezdbsnl.html

Swift .......... 15
来源：http://hz.nwbrower.top/gttmcptkxe.html

Lua ............ 10
来源：http://hz.xinyue.icu/gtpqfretlg.html

Perl ........... 10
来源：http://hz.jqgufenzy.top/gtzipqgnca.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gtbjpncify.html

------------------------------------
来源：http://hz.hnqzz.top/gtgkmdvokm.html

合计 ........... 2106 条
来源：http://hz.hysaishi.cn/gtcmrndxhq.html

按章节统计：
来源：http://hz.bjfxy.top/gtbxeuqmbc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.meibo888.top/gtnuockkwu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtwznliupd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtwprqfywx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gtrgqbudry.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jianghu66.top/gtkivvyvig.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtipghfcfo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtvevgijsb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtrwpxhbrk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.pycfn.com/gtjmuolloh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gtvhpuzfyi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gthsrwvdbb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gteklvmvuz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtkxeqhiov.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gttijyopxu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cucudq.cn/gtzwaxisdd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtgxultjab.html

Q SQL 专题                              90
来源：http://hz.yj202588.top/gtprmpuddy.html

R Bash 专题                             80
来源：http://hz.yueranfly.top/gtyxpcuadv.html

S C / C++ 专题                          60
来源：http://hz.ppjwa.cn/gtiokltpkj.html

T 其他语言补充                          60
来源：http://hz.cheryme.top/gtkhdnxtkl.html

U 高频实用片段                         120
来源：http://hz.0kj1m.cn/gthbroiryt.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gthgtjgsyg.html

合计                                  2106 条
来源：http://hz.tian-w.cn/gtgomdmazy.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtfijdkijj.html

使用提醒
来源：http://hz.cheryme.top/gtrcogowlf.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtvkkpgdlg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtzyhnvwfh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zhixingplan.top/gtavtxorif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hongshengwenyu.top/gtuurezuqd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.dianchejie.cn/gtoaisjmop.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xinyue.icu/gtnafubcvz.html

—— 文件结束 ——
来源：http://hz.jinyuanbaomall.cn/gtrmjoiszu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpvscszhq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yuanzhike.top/gtidhgysxe.html

Common Programming Examples Cheat Book
来源：http://hz.ydjk.org.cn/gtpwfmyhga.html

================================================================================
来源：http://hz.guannengcc.top/gteotctwvb.html

【收录内容】
来源：http://hz.birdmap.top/gtsqcuqxoz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daria6918.cn/gtndisrxjv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jinyuanbaomall.cn/gtjihpkwzc.html

SQL · Bash · C · C++
来源：http://hz.zhoulong.xyz/gtjfduzwoo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinyuanbaomall.cn/gtyuxbtzla.html

【使用说明】
来源：http://hz.guowangkeji.top/gtnuzumdmb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hammf.cn/gtqzuadwyh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shangyingyoupin.top/gtlrgaztdy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shuidangran.top/gtwspqexgo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.daria6918.cn/gttccjeyav.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.chenjidiqi.icu/gtrnbjnadq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.birdmap.top/gtdvbtsnaf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj20258.top/gtkmohvgqq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.nwbrower.top/gtkverpivs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ppjwa.cn/gtvolmsztx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cqqwz.cn/gtjllbpljq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.bjfxy.top/gtxvntxvjl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aizwys.cn/gtlkxrchlg.html

【文件统计】
来源：http://hz.52xcode.cn/gtxysxlfzr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.tanke756.top/gtfmsxxldi.html

--------------------------------------------------------------------------------
来源：http://hz.ybcxt.top/gtwmmjxsjx.html

目  录
来源：http://hz.dianchejie.cn/gtrjcfuyky.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtnxkifrvq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtxodzrktv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtvyutjkpr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtxmetkfoa.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.chenzaomai.com/gtdrthfkux.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jlsjyb.cn/gtiudpqhge.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.quarkkingdee.top/gtulbxnchx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtpiftkifh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenjidiqi.icu/gterehsccc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtnngqrxmu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.fengsongda.top/gtmurhvniq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gttlpwuvhl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258.top/gtaokcqapk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtdsatljer.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shangyingyoupin.top/gteltfolnw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj20258888.top/gthppxaeeb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gttgpuzlzn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shzxlz.cn/gtvqmxxzll.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.iojbl.cn/gtixsatdca.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zhiwuduotai.top/gtzsykxisa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtfidfnnei.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gttdbyccro.html

================================================================================
来源：http://hz.guannengcc.top/gtnccplphe.html

A. 基础语法与类型
来源：http://hz.zdqjudy.top/gtcmshngru.html

================================================================================
来源：http://hz.fzhhl.top/gtxxjlmoem.html

[A01] Hello World
来源：http://hz.wangshuangyany.cn/gtozccbfzv.html

Py:   print("Hello, World!")
来源：http://hz.mhx1999.top/gtjswsxowo.html

PHP:  echo "Hello, World!";
来源：http://hz.ywan-chungtsiang.top/gtdmhjercm.html

JS:   console.log("Hello, World!");
来源：http://hz.aibaodan.cn/gtznkgwvww.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.bjfxy.top/gtxigdbpfq.html

Java: System.out.println("Hello, World!");
来源：http://hz.hnxiangtu.top/gtrlzbfjfl.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.svipenyu.cn/gtihkuhuef.html

Ruby: puts "Hello, World!"
来源：http://hz.zhiwuduotai.top/gtnjnvrtdn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gthnvuioth.html

[A02] 变量声明与赋值
来源：http://hz.shzxlz.cn/gtizbzwqyb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.tian-w.cn/gtnleomxyb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sxryk.cn/gtriofubon.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuetiantiany.cn/gtxswjjync.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.fengsongda.top/gtgmndjorh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtjsqzcjqp.html

Go:   name := "Alex"; age := 20
来源：http://hz.snrcjt.cn/gtpqnypjfl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.kuanghao11.cn/gtwnfkbiia.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.svipenyu.cn/gtbrcezyzs.html

[A03] 常量定义
来源：http://hz.gaohongyu789.top/gtzthfabna.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.feifeiyinyue.top/gtyvgmohon.html

PHP:  const PI = 3.14159;
来源：http://hz.yvedp.cn/gtkltjyfah.html

JS:   const PI = 3.14159;
来源：http://hz.ppjwa.cn/gtovnshhbv.html

TS:   const PI: number = 3.14159;
来源：http://hz.fzhhl.top/gtubquhter.html

Java: static final double PI = 3.14159;
来源：http://hz.tian-w.cn/gtjmouvfjl.html

Go:   const PI = 3.14159
来源：http://hz.tian-w.cn/gtqznezdee.html

Ruby: PI = 3.14159
来源：http://hz.wangshuangyany.cn/gtoenenbge.html

C#:   const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtfrzglhsh.html

[A04] 判断变量类型
来源：http://hz.bjfxy.top/gtkrpbccnt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aibaodan.cn/gtdtcvnbqb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gtdzobnwkn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.dashuyun.cn/gtdatvmadl.html

TS:   typeof x; x instanceof Date
来源：http://hz.ywan-chungtsiang.top/gtuzxzitfb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cashguo.top/gtjzlgackl.html


<!-- 参考信息 -->