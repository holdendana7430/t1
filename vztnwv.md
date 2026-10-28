代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.aibaodan.cn/gtfdfovzds.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.bjfxy.top/gtwzbvsycb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yonumen.top/gtyxepzmyn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ehwqpu.com/gthjzixtdr.html

[U43] PHP：声明命名空间
来源：http://hz.hnqzz.top/gtdopvevll.html

namespace App\Http;
来源：http://hz.xingfuxueyuan.xyz/gtvmwzswnl.html

[U44] PHP：开启严格类型
来源：http://hz.sweek.top/gthtjtadvo.html

declare(strict_types=1);
来源：http://hz.guowangkeji.top/gtutdybfmj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sysykeji.top/gtacbkylvc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtbnbazago.html

[U46] PHP：可空类型
来源：http://hz.xylfe.cn/gtjzzcpeuz.html

?string $name = null
来源：http://hz.jqgfzy.top/gtzhpusuhh.html

[U47] PHP：联合类型
来源：http://hz.pycfn.com/gthwoikxbw.html

int|string $id
来源：http://hz.vqdsnc.cn/gthgkppxcj.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtotvzuhgd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.smart0.xyz/gtwbwilxsm.html

[U49] PHP：只读属性
来源：http://hz.sysykeji.top/gtpbnimqiq.html

public readonly string $name
来源：http://hz.gogol.net.cn/gtfamqkzwk.html

[U50] PHP：构造器属性提升
来源：http://hz.tanke756.top/gtkqmjpwau.html

public function __construct(private int $id) {}
来源：http://hz.chenjidiqi.icu/gtgbakbzyu.html

[U51] PHP：数组解构
来源：http://hz.nanxuanxn.top/gtplkejzcm.html

[$a, $b] = $arr;
来源：http://hz.sweek.top/gtwvmsvnpw.html

[U52] PHP：箭头函数
来源：http://hz.jianghu66.top/gtyeyjzxuv.html

$double = fn($x) => $x * 2;
来源：http://hz.hnxiangtu.top/gtwgumwnmv.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtccpiirac.html

$v = $a ?? $b ?? "default";
来源：http://hz.jianghu66.top/gtvnondeoq.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangkeji.top/gtvkalevcz.html

$obj?->method()
来源：http://hz.andypj.xyz/gtywvcgefu.html

[U55] PHP：match 表达式
来源：http://hz.hywenlv.cn/gtzxtbpllk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.guannengcc.top/gtvnllawap.html

[U56] PHP：命名参数
来源：http://hz.svipenyu.cn/gtghmzypli.html

f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtaikqlfje.html

[U57] PHP：字符串插值
来源：http://hz.pycfn.com/gtzwkwlwla.html

"值: {$a}"
来源：http://hz.yvedp.cn/gtcevxhpck.html

[U58] PHP：数组三件套
来源：http://hz.sysykeji.top/gtfubcuecf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gotoacloud.top/gtcixeqfwz.html

[U59] PHP：自定义排序
来源：http://hz.52xcode.cn/gtslsdblre.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtcvppyieb.html

[U60] PHP：JSON 编解码
来源：http://hz.vqdsnc.cn/gtnqgoaycs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gteedcswcj.html

[U61] PHP：正则
来源：http://hz.316326.xyz/gtqpnhndtq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gttmxscavg.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtbqgypsls.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenzaomai.com/gtofoumlct.html

[U63] PHP：文件读写
来源：http://hz.dashuyun.cn/gtputaofwl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tanke756.top/gtqoujxwvu.html

[U64] PHP：目录遍历
来源：http://hz.sweek.top/gtxhdcafpx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ybcxt.top/gtztgfjgng.html

[U65] PHP：会话
来源：http://hz.xuanzx.com/gtxjrkfnac.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtjzgygslz.html

[U66] PHP：设置 Cookie
来源：http://hz.xziqi.cn/gtdilpbveu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.mhx1999.top/gtwqxwowli.html

[U67] PHP：处理文件上传
来源：http://hz.xingfuxueyuan.xyz/gtxbrtafwe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jianghu66.top/gtinibcois.html

[U68] PHP：PDO 连接
来源：http://hz.fzhhl.top/gtifkazunc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.kuanghao11.cn/gtjvfqdyzy.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxuanxn.top/gtgtxicqxk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtpkrzmzzl.html

[U70] PHP：PDO 事务
来源：http://hz.gzhubu.top/gtabzafsgm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cqqwz.cn/gttfycyknj.html

[U71] PHP：抛出异常
来源：http://hz.jqgufenzy.top/gtibpustgz.html

throw new RuntimeException("失败", 500);
来源：http://hz.nwbrower.top/gtdhvpntzy.html

[U72] PHP：写错误日志
来源：http://hz.bjfxy.top/gtjcaaormf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yuxming.cn/gtyobptszh.html

[U73] PHP：读取 ini 配置
来源：http://hz.gogol.net.cn/gtldtgnjpk.html

parse_ini_file("config.ini", true)
来源：http://hz.zhoulong.xyz/gtnwxgvxol.html

[U74] PHP：读取环境变量
来源：http://hz.zhiwuduotai.top/gtmaxnsedp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sufxvd.cn/gtcjfqxuae.html

[U75] PHP：依赖注入
来源：http://hz.kuanghao11.cn/gtlrbnxjth.html

composer require psr/container
来源：http://hz.kuanghao11.cn/gtzxktoiym.html

[U76] PHP：简单路由
来源：http://hz.snrcjt.cn/gtrictrwdz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yangfankeji.com/gtdvhfiafl.html

[U77] PHP：模板渲染
来源：http://hz.zycfv.cn/gtqsyhchwj.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtpkgidhfj.html

[U78] PHP：单元测试
来源：http://hz.nanxinkj.top/gtlflcluuo.html

composer require --dev phpunit/phpunit
来源：http://hz.yj20258.top/gtbaihxlvs.html

[U79] PHP：静态分析
来源：http://hz.haohaochexian.top/gtnivtiewi.html

composer require --dev phpstan/phpstan
来源：http://hz.zhaomingkeji.xyz/gtwyeemxyg.html

[U80] PHP：代码规范修复
来源：http://hz.xylfe.cn/gtlbadaoes.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sxryk.cn/gtixgoyxfx.html

[U81] JS：初始化项目
来源：http://hz.gaohongyu789.top/gthqxslpfc.html

npm init -y;  npm i express
来源：http://hz.xuetiantiany.cn/gtsgybiqyq.html

[U82] JS：package.json 脚本
来源：http://hz.ybcxt.top/gtkmolgvmv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.wangshuangyany.cn/gtxxfriuek.html

[U83] JS：ES Module 导入导出
来源：http://hz.316326.xyz/gtmonyfcdf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtgtwyvvdr.html

[U84] JS：CommonJS 写法
来源：http://hz.chenzaomai.com/gtyafgopjw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cqqwz.cn/gtoaquwfrt.html

[U85] JS：可选链
来源：http://hz.ydjk.org.cn/gtbynrngtf.html

a?.b?.c
来源：http://hz.jinqigfzy.top/gtoqfxaxws.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gtvsgkjhpv.html

a ?? b
来源：http://hz.yongpay.top/gtuylcquoi.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtlwcnmqqp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jqgfzy.top/gtxqhqwiee.html

[U88] JS：对象展开合并
来源：http://hz.xziqi.cn/gteslzidzc.html

{ ...a, ...b }
来源：http://hz.shzxlz.cn/gtelyrqrgb.html

[U89] JS：数组去重
来源：http://hz.aizwys.cn/gtavgqqilv.html

[...new Set(arr)]
来源：http://hz.yonumen.top/gtitkmvvcf.html

[U90] JS：数字数组排序
来源：http://hz.yangfankeji.com/gtewgedubx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtwbenkszq.html

[U91] JS：对象键值遍历
来源：http://hz.nwbrower.top/gtxkrxalvw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangdashe.top/gtjchsdogf.html

[U92] JS：深拷贝
来源：http://hz.jqgfzy.top/gtypscrhjt.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtcqkmyxjz.html

[U93] JS：模板字符串
来源：http://hz.iojbl.cn/gtsngvzsot.html

`共 ${n} 条`
来源：http://hz.snrcjt.cn/gthrvlxwwt.html

[U94] JS：箭头函数
来源：http://hz.xuetiantiany.cn/gtggpzvpet.html

const double = x => x * 2;
来源：http://hz.ydzc1.top/gtjqqxndbx.html

[U95] JS：Promise 包装
来源：http://hz.yj20258.top/gtzadtnofc.html

new Promise((resolve, reject) => {})
来源：http://hz.chenlongwang.top/gthxeygaxz.html

[U96] JS：async/await 与异常
来源：http://hz.cucudq.cn/gtumqixqvi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtatmfcfzd.html

[U97] JS：并发请求
来源：http://hz.mhx1999.top/gtfcvrshld.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtecapzguw.html

[U98] JS：fetch 带 JSON
来源：http://hz.zycfv.cn/gtibxpzsnz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cdnleiting.top/gtequtclbi.html

[U99] JS：事件监听
来源：http://hz.fzhhl.top/gtrrstevbb.html

el.addEventListener("click", e => {})
来源：http://hz.hywenlv.cn/gtqlcddftx.html

[U100] JS：DOM 查询
来源：http://hz.ehwqpu.com/gtusogodoo.html

document.querySelector(".item")
来源：http://hz.chenjidiqi.icu/gtptalcjnb.html

[U101] JS：classList 操作
来源：http://hz.nwbrower.top/gtnvdehjwv.html

el.classList.toggle("active")
来源：http://hz.316326.xyz/gtugsiroeu.html

[U102] JS：本地存储
来源：http://hz.zhiwuduotai.top/gtjmoyjmes.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tanke756.top/gtsrtlehux.html

[U103] JS：定时器
来源：http://hz.yuanzhike.top/gtorrrwzcn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yangfankeji.com/gtyiltkqbq.html

[U104] JS：防抖
来源：http://hz.shangyingyoupin.top/gtqqxhgemz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtgdakhcdm.html

[U105] JS：节流
来源：http://hz.shzxlz.cn/gtknrfaoiv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.iojbl.cn/gtlzuofbap.html

[U106] JS：日期格式化
来源：http://hz.jqgufenzy.top/gtpysyrxdn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.daria6918.cn/gtenxkrlfy.html

[U107] JS：数字千分位
来源：http://hz.feifeiyinyue.top/gtaihhhlkh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cashguo.top/gtucquonus.html

[U108] JS：随机整数
来源：http://hz.jyoumei.cn/gtwwrknamg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtjziyagds.html

[U109] JS：数组分组
来源：http://hz.xziqi.cn/gtstmkivzc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gteygcyuly.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtrdhzloai.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dashuyun.cn/gtbmjwhkct.html

[U111] JS：对象转 Map
来源：http://hz.jinyuanbaomall.cn/gtxsxljpss.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gtbmyizduu.html

[U112] JS：字符串补位
来源：http://hz.yj20258888.top/gtncpzwqcd.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtjgkekofu.html

[U113] JS：正则替换全部
来源：http://hz.cucudq.cn/gtlzuatbsf.html

s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtpzpdiqus.html

[U114] JS：JSON 深比较
来源：http://hz.c1oappe.top/gtginzqthz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtcwxlcphz.html

[U115] JS：生成 UUID
来源：http://hz.chenzaomai.com/gtfuzqnyrh.html

crypto.randomUUID()
来源：http://hz.havefunace.top/gtkkohawjy.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtwqjjpoma.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yongpay.top/gtwhfchnpx.html

[U117] JS：单元测试
来源：http://hz.yj202588.top/gtdmnnkhaa.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtamekevmt.html

[U118] JS：开发服务器
来源：http://hz.svipenyu.cn/gtpulmlysk.html

npm i -D vite;  npx vite
来源：http://hz.yueranfly.top/gtlotyifmz.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtcqcxxjpc.html

npx vite build
来源：http://hz.52xcode.cn/gtaomeumue.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hywenlv.cn/gtucxeoauc.html

import.meta.env.VITE_API_URL
来源：http://hz.sxryk.cn/gtkjlpphrh.html

================================================================================
来源：http://hz.cucudq.cn/gtuvgkehuc.html

统计汇总
来源：http://hz.smart0.xyz/gtilhmtjyo.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfflynhva.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtdzwwajbe.html

Python ......... 252
来源：http://hz.nanxinkj.top/gttnvfjlop.html

PHP ............ 252
来源：http://hz.hfpthk.cn/gttytxlucx.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gthluqaatk.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtjfdegtch.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtkkdlmlqt.html

Go ............. 212
来源：http://hz.c1oappe.top/gtvvpwrmln.html

Ruby ........... 212
来源：http://hz.gotoacloud.top/gtuonizeor.html

C# ............. 212
来源：http://hz.ehwqpu.com/gtgxndpzsy.html

C .............. 30
来源：http://hz.redwolf501.top/gtgowgeccs.html

C++ ............ 30
来源：http://hz.shangyingyoupin.top/gtmluuwjhm.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtnqouluoq.html

Bash ........... 80
来源：http://hz.guowangkeji.top/gtmghqpvlz.html

Kotlin ......... 15
来源：http://hz.wangdashe.top/gtzkepwgfg.html

Swift .......... 15
来源：http://hz.quarkkingdee.top/gtwasfwovo.html

Lua ............ 10
来源：http://hz.wangdashe.top/gthlbppxdy.html

Perl ........... 10
来源：http://hz.mhx1999.top/gtqgrfngzu.html

Scala .......... 10
来源：http://hz.cdnleiting.top/gtsvyvisjo.html

------------------------------------
来源：http://hz.jianghu66.top/gtmwsalnue.html

合计 ........... 2106 条
来源：http://hz.birdmap.top/gtifbdcbgb.html

按章节统计：
来源：http://hz.yonumen.top/gttysbmqde.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtvvhalohk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtxyzawwoc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtksuinilh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtwrbevbfq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hfpthk.cn/gtkepiinhu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gaohongyu789.top/gtpvczxgqk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtxjwqfwig.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ywan-chungtsiang.top/gtkuflowie.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtujywlxuz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtmqpcppgd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhoulong.xyz/gtjwpmxdrq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtwrpngzgo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtvqsdheni.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtysffooct.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgfzy.top/gtvxwwvylm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gttauhcuru.html

Q SQL 专题                              90
来源：http://hz.dianchejie.cn/gtgogsdwik.html

R Bash 专题                             80
来源：http://hz.yvedp.cn/gtpvqkqbbf.html

S C / C++ 专题                          60
来源：http://hz.guannengcc.top/gtvwpaaeaf.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtakmskjdn.html

U 高频实用片段                         120
来源：http://hz.feifeiyinyue.top/gtctqxonoy.html

------------------------------------
来源：http://hz.zhengqikj.top/gtgzebdukm.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtftfwobpt.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtwethilof.html

使用提醒
来源：http://hz.aibaodan.cn/gtcnyrdwqy.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtzwljmkxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.smart0.xyz/gtggpocdyc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuxming.cn/gtwzdnbseo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.wangdashe.top/gtxinjyihn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xuanzx.com/gtirhiwsht.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tianlin.xyz/gtlzmvxigv.html

—— 文件结束 ——
来源：http://hz.jiagoushi.top/gtesyaavzz.html

================================================================================
来源：http://hz.wangdashe.top/gtabqdopol.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zdqjudy.top/gtwawxaiee.html

Common Programming Examples Cheat Book
来源：http://hz.jqgufenzy.top/gtdshmjxyu.html

================================================================================
来源：http://hz.xylfe.cn/gtfoukupgv.html

【收录内容】
来源：http://hz.ywan-chungtsiang.top/gtkxrptbdu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.snrcjt.cn/gtnplvsjbs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtakmqecbj.html

SQL · Bash · C · C++
来源：http://hz.vqdsnc.cn/gtkznxrqro.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cheryme.top/gtelpxssuu.html

【使用说明】
来源：http://hz.snrcjt.cn/gtwrlprntr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtjhnbbsfp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shanyushiyangkeji.top/gtnzcutepx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenlongwang.top/gtkqdluntw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.andypj.xyz/gtzvosgcfq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxinkj.top/gtyeldzzgd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258.top/gttjjhabpu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.tanke756.top/gtvuczzmia.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.bjfxy.top/gtqxbvwcep.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtscjzuttl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hfpthk.cn/gtpjqkbnkf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daxiang520.top/gthjdzikhw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hongshengwenyu.top/gtcuckckvi.html

【文件统计】
来源：http://hz.nanxinkj.top/gtrqkltzhl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.aizwys.cn/gtfcukccpq.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtxjminxgu.html

目  录
来源：http://hz.0kj1m.cn/gtxgflklhz.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtildbvasn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xuetiantiany.cn/gtvqpuepaj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xinyue.icu/gtzqbebaxh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.dianchejie.cn/gtwdzfynqy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ydjk.org.cn/gtnyxbfjlx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zycfv.cn/gtmpogaygv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shzxlz.cn/gtsksllcwp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yongpay.top/gtzocvakyh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtkqcsdcmf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtymiajngc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sysykeji.top/gtcnjtkctw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtsxvkxaqj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtluuyihpb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtkcahpepp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sweek.top/gtlbngjbsp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sweek.top/gtlyjbbequ.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtafgzgpuo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gzhubu.top/gttxjyciri.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ppjwa.cn/gtjsyquiim.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.chenzaomai.com/gtcxavnavd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtxdjijycy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtbcugfnsn.html

================================================================================
来源：http://hz.cdnleiting.top/gtmpkierpw.html

A. 基础语法与类型
来源：http://hz.svipenyu.cn/gtkvuniefi.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdhgpdkqh.html

[A01] Hello World
来源：http://hz.zhixingplan.top/gtfsvxpize.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gttdqnszar.html

PHP:  echo "Hello, World!";
来源：http://hz.hfpthk.cn/gtmlhivdgo.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtdhaoyjzl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xylfe.cn/gtbitbvixe.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj202588.top/gtdfkpvjjr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.c1oappe.top/gtgnzdfmsq.html

Ruby: puts "Hello, World!"
来源：http://hz.jiagoushi.top/gtmcbsclxq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtwysqiwgv.html

[A02] 变量声明与赋值
来源：http://hz.svipenyu.cn/gtqpvijoom.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.guannengcc.top/gtnoikmhrc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jqgufenzy.top/gtwbvkgepk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.wangdashe.top/gtcrdiphgx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ehwqpu.com/gtgutedfnh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.aizwys.cn/gtcvqrkxbq.html

Go:   name := "Alex"; age := 20
来源：http://hz.ybcxt.top/gtnsxhwflg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.snrcjt.cn/gtdtbwxpdu.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtfqprqzbb.html

[A03] 常量定义
来源：http://hz.sysykeji.top/gttljqwlau.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.mhx1999.top/gtxplowwlm.html

PHP:  const PI = 3.14159;
来源：http://hz.ybcxt.top/gtuplthsrs.html

JS:   const PI = 3.14159;
来源：http://hz.yvedp.cn/gtpvnuqmbc.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtajfdunue.html

Java: static final double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtdypkjoph.html

Go:   const PI = 3.14159
来源：http://hz.ydzc1.top/gtvpdxgahc.html

Ruby: PI = 3.14159
来源：http://hz.hnxiangtu.top/gtxognqvjh.html

C#:   const double PI = 3.14159;
来源：http://hz.cheryme.top/gtwyexsvhp.html

[A04] 判断变量类型
来源：http://hz.ivvv.top/gtvdzehqsv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.wangdashe.top/gtbrgaawwi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.gogol.net.cn/gtzzuxgmvx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cdnleiting.top/gtipyqbkth.html

TS:   typeof x; x instanceof Date
来源：http://hz.xuetiantiany.cn/gthbphhpvt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.smart0.xyz/gtdveedqdu.html


<!-- 参考信息 -->