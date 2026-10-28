代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.snrcjt.cn/gtewlpwmzc.html

namespace App\Http;
来源：http://hz.jinghuilouyu.cn/gtrkapvosn.html

[U44] PHP：开启严格类型
来源：http://hz.jqgfzy.top/gtqkpyjjxq.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtujuykuvh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shuidangran.top/gtfaqrilwi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtytvoictb.html

[U46] PHP：可空类型
来源：http://hz.mhx1999.top/gtcrktqfnj.html

?string $name = null
来源：http://hz.cqqwz.cn/gttlphzxrn.html

[U47] PHP：联合类型
来源：http://hz.0kj1m.cn/gtwqlrzpns.html

int|string $id
来源：http://hz.wangdashe.top/gtgwnhhaku.html

[U48] PHP：纯枚举
来源：http://hz.jlsjyb.cn/gtpwliqbig.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aibaodan.cn/gtlelidcfn.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtjdobbexk.html

public readonly string $name
来源：http://hz.316326.xyz/gtvmsroldm.html

[U50] PHP：构造器属性提升
来源：http://hz.xuanzx.com/gtvywrelzl.html

public function __construct(private int $id) {}
来源：http://hz.gogol.net.cn/gttvhmwabw.html

[U51] PHP：数组解构
来源：http://hz.pengpengdd.cyou/gtyavlajwk.html

[$a, $b] = $arr;
来源：http://hz.nwbrower.top/gtzjygnqnf.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtqiguepzr.html

$double = fn($x) => $x * 2;
来源：http://hz.havefunace.top/gtlhhurqfr.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gtoypnhftn.html

$v = $a ?? $b ?? "default";
来源：http://hz.ywan-chungtsiang.top/gtmblxtgtf.html

[U54] PHP：空安全调用
来源：http://hz.gzhubu.top/gttlzwkhog.html

$obj?->method()
来源：http://hz.fengsongda.top/gtugkuvhnt.html

[U55] PHP：match 表达式
来源：http://hz.cucudq.cn/gtsqzpliqr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.9152youxi.cn/gtrqgmfapn.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gtytdkendd.html

f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtgpwotvbi.html

[U57] PHP：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtwusdbghv.html

"值: {$a}"
来源：http://hz.ydjk.org.cn/gtcrjbvdmo.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtceyuafba.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pycfn.com/gtxudvtxjx.html

[U59] PHP：自定义排序
来源：http://hz.gotoacloud.top/gtocigtytx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtdvjjuulu.html

[U60] PHP：JSON 编解码
来源：http://hz.hammf.cn/gtszwqtapc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jyoumei.cn/gtvztkwcnl.html

[U61] PHP：正则
来源：http://hz.gogol.net.cn/gtyeyzwchu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jlsjyb.cn/gtwutvwvxy.html

[U62] PHP：日期对象
来源：http://hz.meibo888.top/gtzyneeaac.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gtopfhexyd.html

[U63] PHP：文件读写
来源：http://hz.svipenyu.cn/gtqpjcxlhr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtefehcunv.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtrmoxvrtl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhengqikj.top/gtndoffjfm.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtbrcujnna.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenjidiqi.icu/gtfozqqdth.html

[U66] PHP：设置 Cookie
来源：http://hz.hywenlv.cn/gtnvnsejdn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tian-w.cn/gtgcbsktwu.html

[U67] PHP：处理文件上传
来源：http://hz.jyoumei.cn/gtbjutuoln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gtiitdhlhz.html

[U68] PHP：PDO 连接
来源：http://hz.wangdashe.top/gtzokdzglr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.havefunace.top/gtebdwgedq.html

[U69] PHP：PDO 预处理
来源：http://hz.havefunace.top/gttvrrklnf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxinkj.top/gtvnswnxsl.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258888.top/gtfmfaycac.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guowangkeji.top/gtobaomkue.html

[U71] PHP：抛出异常
来源：http://hz.andypj.xyz/gtnyzbovrw.html

throw new RuntimeException("失败", 500);
来源：http://hz.jqgfzy.top/gtgvvvcdho.html

[U72] PHP：写错误日志
来源：http://hz.cashguo.top/gtldbkbdui.html

error_log("失败: " . $e->getMessage());
来源：http://hz.havefunace.top/gtmwvlpqlu.html

[U73] PHP：读取 ini 配置
来源：http://hz.haohaochexian.top/gtrgygogxs.html

parse_ini_file("config.ini", true)
来源：http://hz.zhaomingkeji.xyz/gtfsanohyq.html

[U74] PHP：读取环境变量
来源：http://hz.yuxming.cn/gtekzhgopq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.chenjidiqi.icu/gtbzhovjfv.html

[U75] PHP：依赖注入
来源：http://hz.meibo888.top/gtaucdwgiq.html

composer require psr/container
来源：http://hz.aizwys.cn/gtyolgidou.html

[U76] PHP：简单路由
来源：http://hz.c1oappe.top/gtukxyicnt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dianchejie.cn/gtgblxpuyq.html

[U77] PHP：模板渲染
来源：http://hz.dashuyun.cn/gtxqbmfsok.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gttykaxton.html

[U78] PHP：单元测试
来源：http://hz.zhaomingkeji.xyz/gtlwshkxix.html

composer require --dev phpunit/phpunit
来源：http://hz.gzhubu.top/gtpcioxqjm.html

[U79] PHP：静态分析
来源：http://hz.tian-w.cn/gtpgekbqny.html

composer require --dev phpstan/phpstan
来源：http://hz.wangshuangyany.cn/gtyutukluw.html

[U80] PHP：代码规范修复
来源：http://hz.xziqi.cn/gtjcbranxo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.0kj1m.cn/gtngzuqbje.html

[U81] JS：初始化项目
来源：http://hz.xingfuxueyuan.xyz/gtumfunkzy.html

npm init -y;  npm i express
来源：http://hz.yueranfly.top/gtluerxqcc.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtysfnvwdk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ywan-chungtsiang.top/gtgtxynzaw.html

[U83] JS：ES Module 导入导出
来源：http://hz.shanyushiyangkeji.top/gtbdnxbgqx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj202588.top/gtskqtocig.html

[U84] JS：CommonJS 写法
来源：http://hz.gotoacloud.top/gtwxinqjgh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xuanzx.com/gtmejeewfd.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gtuvcohdrf.html

a?.b?.c
来源：http://hz.ehwqpu.com/gtfucfufvf.html

[U86] JS：空值合并
来源：http://hz.xuetiantiany.cn/gtubztkfcb.html

a ?? b
来源：http://hz.chenlongwang.top/gtlyyknbdx.html

[U87] JS：解构默认值
来源：http://hz.pycfn.com/gtjfurbtbd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yangfankeji.com/gtubhdzlsj.html

[U88] JS：对象展开合并
来源：http://hz.cqqwz.cn/gthuaqjaqm.html

{ ...a, ...b }
来源：http://hz.quarkkingdee.top/gtbhdnuifw.html

[U89] JS：数组去重
来源：http://hz.gaohongyu789.top/gtiznxftzz.html

[...new Set(arr)]
来源：http://hz.shzxlz.cn/gtnxuvhwjc.html

[U90] JS：数字数组排序
来源：http://hz.yuxming.cn/gtxtkdvcxg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtmcemcfcc.html

[U91] JS：对象键值遍历
来源：http://hz.dashuyun.cn/gtmetirtac.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yonumen.top/gttjzmcrkg.html

[U92] JS：深拷贝
来源：http://hz.c1oappe.top/gtsjnllbep.html

structuredClone(obj)
来源：http://hz.yongpay.top/gtyoiipgzb.html

[U93] JS：模板字符串
来源：http://hz.svipenyu.cn/gtnsxpmemt.html

`共 ${n} 条`
来源：http://hz.cdnleiting.top/gtmuphcmzu.html

[U94] JS：箭头函数
来源：http://hz.yj202588.top/gtugtitcar.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gttxkxhyap.html

[U95] JS：Promise 包装
来源：http://hz.52xcode.cn/gtiuatjuiz.html

new Promise((resolve, reject) => {})
来源：http://hz.aibaodan.cn/gtrfiivbom.html

[U96] JS：async/await 与异常
来源：http://hz.cucudq.cn/gtkwhapnep.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtyfmepfbq.html

[U97] JS：并发请求
来源：http://hz.nanxuanxn.top/gtlwnrqqyk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtijfeuzry.html

[U98] JS：fetch 带 JSON
来源：http://hz.c1oappe.top/gtissfcnqv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shanyushiyangkeji.top/gtohuqcqod.html

[U99] JS：事件监听
来源：http://hz.shzxlz.cn/gteowffbts.html

el.addEventListener("click", e => {})
来源：http://hz.xuanzx.com/gtmwdcxftx.html

[U100] JS：DOM 查询
来源：http://hz.aibaodan.cn/gtfkvcvqqt.html

document.querySelector(".item")
来源：http://hz.xingfuxueyuan.xyz/gtsmlxdgvu.html

[U101] JS：classList 操作
来源：http://hz.xuanzx.com/gtmnvbbbry.html

el.classList.toggle("active")
来源：http://hz.nwbrower.top/gtzmhcomyb.html

[U102] JS：本地存储
来源：http://hz.quarkkingdee.top/gtmdeicmfb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ybcxt.top/gtsrtaaelf.html

[U103] JS：定时器
来源：http://hz.hnxiangtu.top/gtinyezxmy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hnxiangtu.top/gtuozfpwcg.html

[U104] JS：防抖
来源：http://hz.xylfe.cn/gtfsplalaz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sxryk.cn/gtwotgtcnh.html

[U105] JS：节流
来源：http://hz.yanxiufei.cn/gtioxsqulb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtbrcfnhdb.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtgrgvwvyp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jianghu66.top/gtwrdpeymi.html

[U107] JS：数字千分位
来源：http://hz.guowangkeji.top/gtkshdtbdh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtsiluyoji.html

[U108] JS：随机整数
来源：http://hz.jinyuanbaomall.cn/gtfncfxigz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtpakvnkop.html

[U109] JS：数组分组
来源：http://hz.c1oappe.top/gtldjhwivp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtqvqukqkg.html

[U110] JS：数组分块
来源：http://hz.jinqigufen.top/gtpqadinqw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shangyingyoupin.top/gtkujtsujq.html

[U111] JS：对象转 Map
来源：http://hz.ppjwa.cn/gtndeukecn.html

new Map(Object.entries(obj))
来源：http://hz.fengsongda.top/gtgjwwzjiy.html

[U112] JS：字符串补位
来源：http://hz.ywan-chungtsiang.top/gtyqjpawol.html

"7".padStart(3, "0")
来源：http://hz.yj20258.top/gtymwqckll.html

[U113] JS：正则替换全部
来源：http://hz.shangyingyoupin.top/gtyzuoqkkb.html

s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gtyjnbamji.html

[U114] JS：JSON 深比较
来源：http://hz.shzxlz.cn/gtztomuazb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.c1oappe.top/gtshdncawg.html

[U115] JS：生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtgipbsqyo.html

crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gtuartscec.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ydzc1.top/gttayweyap.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cheryme.top/gthnljpjsv.html

[U117] JS：单元测试
来源：http://hz.zhiwuduotai.top/gtaacqinsm.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gtjkvymfpi.html

[U118] JS：开发服务器
来源：http://hz.chenlongwang.top/gtyjpppnhf.html

npm i -D vite;  npx vite
来源：http://hz.jinghuilouyu.cn/gtcwpdfgxt.html

[U119] JS：生产构建
来源：http://hz.zhiwuduotai.top/gtobmxetfg.html

npx vite build
来源：http://hz.ywan-chungtsiang.top/gtlziovasg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yangfankeji.com/gtkpuhqhom.html

import.meta.env.VITE_API_URL
来源：http://hz.tanke756.top/gtgulvqodi.html

================================================================================
来源：http://hz.ivvv.top/gtcwajkrah.html

统计汇总
来源：http://hz.gotoacloud.top/gtzgufjrwl.html

================================================================================
来源：http://hz.cdnleiting.top/gtodyurazl.html

按语言统计（条）：
来源：http://hz.yongpay.top/gteramdoja.html

Python ......... 252
来源：http://hz.shanyushiyangtech.top/gtklkaakiw.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtkknepzqv.html

JavaScript ..... 252
来源：http://hz.hnqzz.top/gthzswawbz.html

TypeScript ..... 212
来源：http://hz.shangyingyoupin.top/gtfsyidkpi.html

Java ........... 212
来源：http://hz.jyoumei.cn/gtzbmhssmz.html

Go ............. 212
来源：http://hz.aizwys.cn/gtrnjwndzm.html

Ruby ........... 212
来源：http://hz.jqgfzy.top/gtukiybpfv.html

C# ............. 212
来源：http://hz.xziqi.cn/gtzmboygjo.html

C .............. 30
来源：http://hz.iojbl.cn/gtjbpcjolh.html

C++ ............ 30
来源：http://hz.nanxinkj.top/gtlcxesndo.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtuwjqotqs.html

Bash ........... 80
来源：http://hz.guannengcc.top/gthnuqrmhd.html

Kotlin ......... 15
来源：http://hz.shangyingyoupin.top/gtwptprgeb.html

Swift .......... 15
来源：http://hz.chenzaomai.com/gtsvoauogv.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gttovmxbaa.html

Perl ........... 10
来源：http://hz.ydzc1.top/gtvctovxeu.html

Scala .......... 10
来源：http://hz.jqgfzy.top/gtxrbgbtcm.html

------------------------------------
来源：http://hz.wangdashe.top/gtvuneaord.html

合计 ........... 2106 条
来源：http://hz.pengpengdd.cyou/gtlfbcnxrc.html

按章节统计：
来源：http://hz.birdmap.top/gtdogihayu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhongyouzk.top/gttkqqwtgg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtnrnpxcxj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtgshtpwaf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ybcxt.top/gtmsdpksst.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jyoumei.cn/gtvlusramk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhiwuduotai.top/gtznghgttq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtjbrfyysx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtsfynmgym.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtelwexxsw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gthznahmkw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtwvmdfdtw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtdfkkowxc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtbpqftllz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangshuangyany.cn/gtppttpotw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.aizwys.cn/gtbqrcbkmq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gttlgxgceo.html

Q SQL 专题                              90
来源：http://hz.jinghuilouyu.cn/gtowxizuqi.html

R Bash 专题                             80
来源：http://hz.jqgfzy.top/gtroxnxmpn.html

S C / C++ 专题                          60
来源：http://hz.jlsjyb.cn/gtodiaxgen.html

T 其他语言补充                          60
来源：http://hz.yj20258.top/gtmvjtbahm.html

U 高频实用片段                         120
来源：http://hz.shanyushiyangkeji.top/gtqmehnqnk.html

------------------------------------
来源：http://hz.mhx1999.top/gtdydsjlon.html

合计                                  2106 条
来源：http://hz.birdmap.top/gtnufyzdac.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtfdoavjov.html

使用提醒
来源：http://hz.yj20258.top/gtgcvbtvxv.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gthxmjvffq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigfzy.top/gtyvjakjhe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtsvomxfai.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fzhhl.top/gtdieznker.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.aizwys.cn/gtiecubvwn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinghuilouyu.cn/gtwvxwtysb.html

—— 文件结束 ——
来源：http://hz.jlsjyb.cn/gtcwyecqkl.html

================================================================================
来源：http://hz.sufxvd.cn/gtmtgomlwn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydjk.org.cn/gtlxosppfl.html

Common Programming Examples Cheat Book
来源：http://hz.zycfv.cn/gtwvvxegjn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwdlyijbp.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtclblkzut.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.fzhhl.top/gtavdrmfxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tanke756.top/gtiqgtgpqu.html

SQL · Bash · C · C++
来源：http://hz.quarkkingdee.top/gtstxpmbsn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.aibaodan.cn/gtraqtzzum.html

【使用说明】
来源：http://hz.52xcode.cn/gtpberlifu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yvedp.cn/gtxechuvsx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jyoumei.cn/gtjatzoelk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tanke756.top/gtnzpikwbg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gthibaufmo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigufen.top/gtzpxsnjls.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.aibaodan.cn/gtjaabluvk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ywan-chungtsiang.top/gtzljjrcil.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.andypj.xyz/gtgsfezlac.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sxryk.cn/gtnvkwzfvh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tian-w.cn/gtadysrpyv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtmmddxbqt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.meibo888.top/gtqcxhmrkf.html

【文件统计】
来源：http://hz.ywan-chungtsiang.top/gtfuezulic.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.52xcode.cn/gtwoukilkz.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtjnasqxde.html

目  录
来源：http://hz.quarkkingdee.top/gtonlblber.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtnazjuyue.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dashuyun.cn/gtsodqskrg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.52xcode.cn/gtwvliaaty.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtthsylgst.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhiwuduotai.top/gtsdgzuncu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shzxlz.cn/gtnlagbnpt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinqigufen.top/gtmcfejyet.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zdqjudy.top/gtkyduwfxm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtokakvpeo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtrdkwoeet.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gtkepkupez.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtompbhsfa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtmazclybl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gttnxhxfze.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sxryk.cn/gtaddnwduv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.quarkkingdee.top/gtcpwgbuqa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtigomdihw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.tanke756.top/gtqjqdfmlp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gtsiwffkww.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.aizwys.cn/gtforvtrjh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtrideduvw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtabixcmrh.html

================================================================================
来源：http://hz.tianlin.xyz/gtxrfmxmrv.html

A. 基础语法与类型
来源：http://hz.iojbl.cn/gtrqaxdaqp.html

================================================================================
来源：http://hz.smart0.xyz/gtsvzlremt.html

[A01] Hello World
来源：http://hz.ehwqpu.com/gtxmzxngas.html

Py:   print("Hello, World!")
来源：http://hz.zhijiandao.cn/gtxdfmqaxc.html

PHP:  echo "Hello, World!";
来源：http://hz.yuxming.cn/gtwzeanghh.html

JS:   console.log("Hello, World!");
来源：http://hz.jianghu66.top/gtixgjsufp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhengqikj.top/gtgcnjblvn.html

Java: System.out.println("Hello, World!");
来源：http://hz.andypj.xyz/gtybxuzywm.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yonumen.top/gtdalnsqod.html

Ruby: puts "Hello, World!"
来源：http://hz.yuxming.cn/gtzecwktpg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenlongwang.top/gtvvflatzd.html

[A02] 变量声明与赋值
来源：http://hz.feifeiyinyue.top/gtpukflhbw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yueranfly.top/gtithftbpa.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yj20258.top/gtqdmlprvg.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtzqvqdtix.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hysaishi.cn/gtmfsnahbb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ppjwa.cn/gtwgrxvlix.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtkpxqhebt.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yonumen.top/gtixjsjpub.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yueranfly.top/gtkaxchicy.html

[A03] 常量定义
来源：http://hz.sufxvd.cn/gtjijwoykv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.aizwys.cn/gttygxpzak.html

PHP:  const PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtgywktvvq.html

JS:   const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtqfdjfwce.html

TS:   const PI: number = 3.14159;
来源：http://hz.jqgfzy.top/gtxlhypvxb.html

Java: static final double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtchnzmxbk.html

Go:   const PI = 3.14159
来源：http://hz.yj20258.top/gtqnmovpwm.html

Ruby: PI = 3.14159
来源：http://hz.sufxvd.cn/gtbftzvbxq.html

C#:   const double PI = 3.14159;
来源：http://hz.mhx1999.top/gtyneyxzqq.html

[A04] 判断变量类型
来源：http://hz.shanyushiyangtech.top/gtdnzwtgjl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gtpettdfhp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.feifeiyinyue.top/gtbnmqfqzw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.guannengcc.top/gtntgdjbga.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtaqutoysu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gtpuezqklg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhongyouzk.top/gtkunaldur.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxinkj.top/gtuejyemwz.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhixingplan.top/gtnybizujo.html

[A05] 整数除法与取模
来源：http://hz.hnxiangtu.top/gtgycwguso.html


<!-- 参考信息 -->