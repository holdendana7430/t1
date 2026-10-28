代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.jinqigfzy.top/gtdqphljpu.html

namespace App\Http;
来源：http://hz.zhengqikj.top/gtbsafpqqn.html

[U44] PHP：开启严格类型
来源：http://hz.pycfn.com/gtjamvrqmc.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gtwtgjepyi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pengpengdd.cyou/gtjcebtubb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtzknlttgm.html

[U46] PHP：可空类型
来源：http://hz.52xcode.cn/gtzinkuuqt.html

?string $name = null
来源：http://hz.yonumen.top/gtqarwcypl.html

[U47] PHP：联合类型
来源：http://hz.kuanghao11.cn/gtogflcwib.html

int|string $id
来源：http://hz.sysykeji.top/gtkphhmcwe.html

[U48] PHP：纯枚举
来源：http://hz.jinqigufen.top/gtaqtnvsjw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtqlpyofin.html

[U49] PHP：只读属性
来源：http://hz.yongpay.top/gtdtkfjgti.html

public readonly string $name
来源：http://hz.mhx1999.top/gtfldivwgc.html

[U50] PHP：构造器属性提升
来源：http://hz.xuanzx.com/gtkijxluzg.html

public function __construct(private int $id) {}
来源：http://hz.yj202588.top/gtbzkkbgcs.html

[U51] PHP：数组解构
来源：http://hz.yj20258.top/gtuirqdjfz.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtkrecwtaa.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtflyhkpmi.html

$double = fn($x) => $x * 2;
来源：http://hz.bjfxy.top/gtxsqapusq.html

[U53] PHP：空合并运算符
来源：http://hz.cucudq.cn/gtjkchwjpa.html

$v = $a ?? $b ?? "default";
来源：http://hz.birdmap.top/gtwtxicdks.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtmeuytnrz.html

$obj?->method()
来源：http://hz.chenlongwang.top/gtpyrbjbki.html

[U55] PHP：match 表达式
来源：http://hz.jinyuanbaomall.cn/gtvvqenaya.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxuanxn.top/gtmxvboccj.html

[U56] PHP：命名参数
来源：http://hz.jqgfzy.top/gtwwjbqxft.html

f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtduasuypm.html

[U57] PHP：字符串插值
来源：http://hz.zhiwuduotai.top/gtwhvoauua.html

"值: {$a}"
来源：http://hz.guowangkeji.top/gtgrkxbttr.html

[U58] PHP：数组三件套
来源：http://hz.dashuyun.cn/gthgdmxlhc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtdaddtgue.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gttsekzbpi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtemxyiidc.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtditbgyji.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hnxiangtu.top/gtcxiejokl.html

[U61] PHP：正则
来源：http://hz.smart0.xyz/gtkfhjipos.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtgrpykbbw.html

[U62] PHP：日期对象
来源：http://hz.sufxvd.cn/gtclhyvcfd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shuidangran.top/gtxmxmippp.html

[U63] PHP：文件读写
来源：http://hz.daxiang520.top/gtidcpjlve.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhiwuduotai.top/gtwascdpmn.html

[U64] PHP：目录遍历
来源：http://hz.meibo888.top/gtaxtvtcsy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hfpthk.cn/gtzledecbo.html

[U65] PHP：会话
来源：http://hz.sweek.top/gtilnbsast.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtrfuxtnid.html

[U66] PHP：设置 Cookie
来源：http://hz.jinghuilouyu.cn/gtswgmgvnf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.316326.xyz/gtvsnzezat.html

[U67] PHP：处理文件上传
来源：http://hz.guowangkeji.top/gtdzjyjaur.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tian-w.cn/gtusjcwfhu.html

[U68] PHP：PDO 连接
来源：http://hz.aizwys.cn/gtufwxqbll.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yvedp.cn/gtvfyoszlb.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtzbewsrtc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gzhubu.top/gtqoqlsbqn.html

[U70] PHP：PDO 事务
来源：http://hz.316326.xyz/gtnvdxkecl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgufenzy.top/gtgvsfphdt.html

[U71] PHP：抛出异常
来源：http://hz.nwbrower.top/gtrbugfljd.html

throw new RuntimeException("失败", 500);
来源：http://hz.sxryk.cn/gtlpnkgoeb.html

[U72] PHP：写错误日志
来源：http://hz.jinqigfzy.top/gtmizuuhak.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtfyabdogz.html

[U73] PHP：读取 ini 配置
来源：http://hz.cdnleiting.top/gttvatrysr.html

parse_ini_file("config.ini", true)
来源：http://hz.fzhhl.top/gtasqfufrk.html

[U74] PHP：读取环境变量
来源：http://hz.quarkkingdee.top/gtjwhpzuns.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hongshengwenyu.top/gtoblcfjfi.html

[U75] PHP：依赖注入
来源：http://hz.zhongyouzk.top/gthqnbdacq.html

composer require psr/container
来源：http://hz.birdmap.top/gtytixjmhn.html

[U76] PHP：简单路由
来源：http://hz.yueranfly.top/gtmpwssouy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ywan-chungtsiang.top/gtxmkwqyql.html

[U77] PHP：模板渲染
来源：http://hz.birdmap.top/gtginumiix.html

composer require twig/twig
来源：http://hz.yj20258.top/gtqfgxruqa.html

[U78] PHP：单元测试
来源：http://hz.feifeiyinyue.top/gtsgzawuet.html

composer require --dev phpunit/phpunit
来源：http://hz.havefunace.top/gtiyqknjip.html

[U79] PHP：静态分析
来源：http://hz.guannengcc.top/gtxecohzlb.html

composer require --dev phpstan/phpstan
来源：http://hz.jianghu66.top/gtvrearipr.html

[U80] PHP：代码规范修复
来源：http://hz.c1oappe.top/gtcgppovqb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xinyue.icu/gtmxtezvkt.html

[U81] JS：初始化项目
来源：http://hz.jqgufenzy.top/gtyyfjhgyi.html

npm init -y;  npm i express
来源：http://hz.zhixingplan.top/gtscawlbmz.html

[U82] JS：package.json 脚本
来源：http://hz.hnqzz.top/gtxcjodtcz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ywan-chungtsiang.top/gtkoxhmaod.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtqxxgybfv.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhixingplan.top/gtaldjrlpc.html

[U84] JS：CommonJS 写法
来源：http://hz.yonumen.top/gtbxgbglyt.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.andypj.xyz/gtycqapcip.html

[U85] JS：可选链
来源：http://hz.jlsjyb.cn/gtjcpefeae.html

a?.b?.c
来源：http://hz.zhongyouzk.top/gttjpddctv.html

[U86] JS：空值合并
来源：http://hz.jqgfzy.top/gtwcgimmoz.html

a ?? b
来源：http://hz.zhixingplan.top/gtlewqqmfm.html

[U87] JS：解构默认值
来源：http://hz.cheryme.top/gtdtkzfxim.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yj202588.top/gtgzpjxodf.html

[U88] JS：对象展开合并
来源：http://hz.ehwqpu.com/gtdggcjbyf.html

{ ...a, ...b }
来源：http://hz.wangdashe.top/gtqtiglrus.html

[U89] JS：数组去重
来源：http://hz.yj202588.top/gtvhrjeoqb.html

[...new Set(arr)]
来源：http://hz.haohaochexian.top/gtyfwccywo.html

[U90] JS：数字数组排序
来源：http://hz.hnqzz.top/gtmrszxgio.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtslvjgjly.html

[U91] JS：对象键值遍历
来源：http://hz.zycfv.cn/gtnahgmers.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gaohongyu789.top/gtwtdqpzvd.html

[U92] JS：深拷贝
来源：http://hz.ydzc1.top/gtoaittngs.html

structuredClone(obj)
来源：http://hz.shzxlz.cn/gtzbyvlccl.html

[U93] JS：模板字符串
来源：http://hz.52xcode.cn/gtvzqtyvfb.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtpfbglmhs.html

[U94] JS：箭头函数
来源：http://hz.birdmap.top/gtskexdojg.html

const double = x => x * 2;
来源：http://hz.shanyushiyangkeji.top/gtoywhltux.html

[U95] JS：Promise 包装
来源：http://hz.zhoulong.xyz/gttuzimstm.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtvnqxcxoy.html

[U96] JS：async/await 与异常
来源：http://hz.birdmap.top/gtwqxixemc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtaopviruj.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangkeji.top/gtgqmqusac.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtgmktpfkb.html

[U98] JS：fetch 带 JSON
来源：http://hz.fzhhl.top/gtkochzkgv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.9152youxi.cn/gtrdchhdiq.html

[U99] JS：事件监听
来源：http://hz.zhaomingkeji.xyz/gtjaklalli.html

el.addEventListener("click", e => {})
来源：http://hz.dashuyun.cn/gtxbvfrhid.html

[U100] JS：DOM 查询
来源：http://hz.zhongyouzk.top/gtyhgumdep.html

document.querySelector(".item")
来源：http://hz.yongpay.top/gtmyzczjpc.html

[U101] JS：classList 操作
来源：http://hz.shanyushiyangtech.top/gtswiwkthy.html

el.classList.toggle("active")
来源：http://hz.quarkkingdee.top/gtijbmmybo.html

[U102] JS：本地存储
来源：http://hz.redwolf501.top/gtvejsggci.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.xuanzx.com/gtjkuvmkuh.html

[U103] JS：定时器
来源：http://hz.aibaodan.cn/gtnfbbixgq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.quarkkingdee.top/gtnpbfojfn.html

[U104] JS：防抖
来源：http://hz.0kj1m.cn/gtkzokccak.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hfpthk.cn/gtxfnumwzs.html

[U105] JS：节流
来源：http://hz.mhx1999.top/gtgjxuyvzz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydzc1.top/gtyhojprwb.html

[U106] JS：日期格式化
来源：http://hz.quarkkingdee.top/gtoxepzbpt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigfzy.top/gtwuflyaoc.html

[U107] JS：数字千分位
来源：http://hz.9152youxi.cn/gtugjnqmut.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xziqi.cn/gtkoxouyqo.html

[U108] JS：随机整数
来源：http://hz.ivvv.top/gtrlmltbne.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtmztodisp.html

[U109] JS：数组分组
来源：http://hz.hammf.cn/gtakiqsqwu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigfzy.top/gtjtwjveus.html

[U110] JS：数组分块
来源：http://hz.guowangkeji.top/gtoyuvhjsm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ppjwa.cn/gtkycbzfvh.html

[U111] JS：对象转 Map
来源：http://hz.xuetiantiany.cn/gtgpwglhop.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gtkedejbig.html

[U112] JS：字符串补位
来源：http://hz.c1oappe.top/gtemvsdjjh.html

"7".padStart(3, "0")
来源：http://hz.xziqi.cn/gttqbdohib.html

[U113] JS：正则替换全部
来源：http://hz.c1oappe.top/gtgsgzsduw.html

s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtekqvinte.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtnyxavqou.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtxoadofhh.html

[U115] JS：生成 UUID
来源：http://hz.zhixingplan.top/gtekfkgfhb.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtpwrtttip.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.kuanghao11.cn/gtkmwsnqtr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jlsjyb.cn/gtxvgzafpi.html

[U117] JS：单元测试
来源：http://hz.316326.xyz/gtfoxqlcjr.html

npm i -D vitest;  npx vitest
来源：http://hz.jlsjyb.cn/gtpcjacrzx.html

[U118] JS：开发服务器
来源：http://hz.yueranfly.top/gtzjvduyac.html

npm i -D vite;  npx vite
来源：http://hz.hnqzz.top/gtiuwwbypq.html

[U119] JS：生产构建
来源：http://hz.0kj1m.cn/gtbxhmskik.html

npx vite build
来源：http://hz.chenjidiqi.icu/gtgqxkjaux.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sweek.top/gtjtomrlfj.html

import.meta.env.VITE_API_URL
来源：http://hz.snrcjt.cn/gtmebzaind.html

================================================================================
来源：http://hz.jqgufenzy.top/gtowkmvfrs.html

统计汇总
来源：http://hz.cheryme.top/gtrmxnmfnr.html

================================================================================
来源：http://hz.gzhubu.top/gtinaxehbm.html

按语言统计（条）：
来源：http://hz.daria6918.cn/gtfwcbxung.html

Python ......... 252
来源：http://hz.yj20258.top/gtyzckqmyf.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtbhgefkit.html

JavaScript ..... 252
来源：http://hz.nanxuanxn.top/gtikrzgqjb.html

TypeScript ..... 212
来源：http://hz.tanke756.top/gtwgyyvwjo.html

Java ........... 212
来源：http://hz.gaohongyu789.top/gtkmughswa.html

Go ............. 212
来源：http://hz.yuxming.cn/gtbbpepkkl.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gtocmsnpzb.html

C# ............. 212
来源：http://hz.aizwys.cn/gtpbszokmm.html

C .............. 30
来源：http://hz.meibo888.top/gtycbupkzq.html

C++ ............ 30
来源：http://hz.andypj.xyz/gtcpkmliuf.html

SQL ............ 90
来源：http://hz.sysykeji.top/gtuadhgfrn.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtycjvazdv.html

Kotlin ......... 15
来源：http://hz.jinghuilouyu.cn/gtdfbgzpbr.html

Swift .......... 15
来源：http://hz.guannengcc.top/gttyoymuus.html

Lua ............ 10
来源：http://hz.cheryme.top/gtifayeuxy.html

Perl ........... 10
来源：http://hz.sufxvd.cn/gtqmoztnfi.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtypolhwbk.html

------------------------------------
来源：http://hz.gotoacloud.top/gtjbtihyaf.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtvrnwpmqo.html

按章节统计：
来源：http://hz.52xcode.cn/gtplohbmzw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtsjppgadm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ppjwa.cn/gtgzcerpuw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.shuidangran.top/gtmuerrigk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shanyushiyangtech.top/gttwwhotaa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhijiandao.cn/gtrjrspvpj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtrfdzozjb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtszttlfgj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xziqi.cn/gtsofopcte.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gtfdhgbifo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtpltuttgr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtbnwdxbcp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtlckdpfpy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangkeji.top/gtfbptknzb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtekgssduc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gtyxujpgxc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.sxryk.cn/gttompjlxj.html

Q SQL 专题                              90
来源：http://hz.vqdsnc.cn/gtpfdfwoon.html

R Bash 专题                             80
来源：http://hz.gogol.net.cn/gtjzqtklug.html

S C / C++ 专题                          60
来源：http://hz.nanxinkj.top/gtinuuuyjg.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtetszmopq.html

U 高频实用片段                         120
来源：http://hz.316326.xyz/gtlzkqmemo.html

------------------------------------
来源：http://hz.ehwqpu.com/gtthykcmmx.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtavcsvxtx.html

--------------------------------------------------------------------------------
来源：http://hz.xingfuxueyuan.xyz/gthzhzrysx.html

使用提醒
来源：http://hz.havefunace.top/gtefntqxvp.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtqiwvjiui.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtpfjzrtho.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.birdmap.top/gtyihbssqy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ehwqpu.com/gtwuodkjry.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxuanxn.top/gtuuyeqnei.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtlgojfnns.html

—— 文件结束 ——
来源：http://hz.dianchejie.cn/gtrmrcmmzj.html

================================================================================
来源：http://hz.ppjwa.cn/gtamhojhuu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxuanxn.top/gtxysaasie.html

Common Programming Examples Cheat Book
来源：http://hz.jiagoushi.top/gtycvzznwj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrfxmceev.html

【收录内容】
来源：http://hz.zhixingplan.top/gtzvwqilap.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.xingfuxueyuan.xyz/gtsvhxpcxh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.andypj.xyz/gtwortdnlt.html

SQL · Bash · C · C++
来源：http://hz.jqgfzy.top/gtnwzcqplj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.aizwys.cn/gtmoucouym.html

【使用说明】
来源：http://hz.yueranfly.top/gtudytuqyx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.haohaochexian.top/gtszwfwydl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xylfe.cn/gtbntsyuud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.mhx1999.top/gtnghainlk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tianlin.xyz/gtxncqckgx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.tian-w.cn/gtamvbprtc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtmcmnhvmz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenlongwang.top/gtaqxoymge.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gaohongyu789.top/gtlmmqgfkv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gtchfraqql.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.chenlongwang.top/gtelrlxkul.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.c1oappe.top/gtfrpwkedp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gaohongyu789.top/gtqillzgrs.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtmqkwihyq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sxryk.cn/gtofwylkhw.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtxcwlybil.html

目  录
来源：http://hz.mhx1999.top/gtpivooxho.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtsmxjkswi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.smart0.xyz/gtxpkkdyqc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gtvcvmqtec.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.birdmap.top/gtbnrrftjr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtixtineos.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgufenzy.top/gtwfbfzdwe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtfbpzyado.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtzlbddxiz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gtkzctabya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtaiyopbjb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gtjatujdku.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gttkwnzsix.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtqgxswyza.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtaxzjtfmn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sweek.top/gtsamnwawv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangtech.top/gtiijoujvh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtcsqxkgkl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yj20258.top/gtmyfwzchv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenjidiqi.icu/gtecaceenq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.svipenyu.cn/gtdcwxmeux.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtxypwofye.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gtuevyszgs.html

================================================================================
来源：http://hz.cashguo.top/gtkxlmaucd.html

A. 基础语法与类型
来源：http://hz.zhaomingkeji.xyz/gtcqesiogg.html

================================================================================
来源：http://hz.meibo888.top/gtjhqndyzu.html

[A01] Hello World
来源：http://hz.yanxiufei.cn/gtpvqtsyfm.html

Py:   print("Hello, World!")
来源：http://hz.hywenlv.cn/gtozkplgdk.html

PHP:  echo "Hello, World!";
来源：http://hz.zhiwuduotai.top/gtngorisbs.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtjjeaprxz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yuanzhike.top/gtvdqaofbn.html

Java: System.out.println("Hello, World!");
来源：http://hz.9152youxi.cn/gtanmlvsvl.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jqgfzy.top/gtmqzicvko.html

Ruby: puts "Hello, World!"
来源：http://hz.hnqzz.top/gthqgrrvbl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtaxjsstnk.html

[A02] 变量声明与赋值
来源：http://hz.sysykeji.top/gtvmsgohup.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gthykiuqvv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yonumen.top/gtbkmmensz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangtech.top/gtzbbutrvi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tianlin.xyz/gtfkzwzakm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtfqtzcbgs.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhongyouzk.top/gtlsjyizvu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinghuilouyu.cn/gtjoxlpunb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.snrcjt.cn/gtnpecuxpp.html

[A03] 常量定义
来源：http://hz.fengsongda.top/gtgzrgwglu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sxryk.cn/gtbdeqpycm.html

PHP:  const PI = 3.14159;
来源：http://hz.jianghu66.top/gtaccjagkm.html

JS:   const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtjbfejqln.html

TS:   const PI: number = 3.14159;
来源：http://hz.nwbrower.top/gtukmbjahr.html

Java: static final double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtkjsdgjgx.html

Go:   const PI = 3.14159
来源：http://hz.yj20258888.top/gtvuvtioix.html

Ruby: PI = 3.14159
来源：http://hz.meibo888.top/gtwleuudko.html

C#:   const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtbghlpcfw.html

[A04] 判断变量类型
来源：http://hz.feifeiyinyue.top/gtcekiqzxb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.shuidangran.top/gthajlcuhh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.fzhhl.top/gttwrkgqrn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jqgfzy.top/gtennzetwk.html

TS:   typeof x; x instanceof Date
来源：http://hz.xuetiantiany.cn/gtvzbbtvat.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.haohaochexian.top/gtkrlrrswo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xingfuxueyuan.xyz/gtgrrpyrcr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yuxming.cn/gtomngcukd.html

C#:   x.GetType().Name; x is int
来源：http://hz.tanke756.top/gtytkkezfz.html

[A05] 整数除法与取模
来源：http://hz.zycfv.cn/gtuluuzfbf.html


<!-- 参考信息 -->