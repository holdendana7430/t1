代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://hz.ybcxt.top/gtfnrepkdq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cdnleiting.top/gtdpkfvncn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.iojbl.cn/gtznijnqmp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuxming.cn/gtmmfpltuz.html

[U43] PHP：声明命名空间
来源：http://hz.jinqigufen.top/gtgfcbmfeu.html

namespace App\Http;
来源：http://hz.yanxiufei.cn/gtiursqgzi.html

[U44] PHP：开启严格类型
来源：http://hz.gotoacloud.top/gtojmkhxod.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtxswgxdes.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gaohongyu789.top/gtisiypgnq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtayxfnjmf.html

[U46] PHP：可空类型
来源：http://hz.chenjidiqi.icu/gtjboetkcr.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtsswmarxi.html

[U47] PHP：联合类型
来源：http://hz.gogol.net.cn/gtrobdzmbz.html

int|string $id
来源：http://hz.hfpthk.cn/gthuqgdxpc.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangtech.top/gtjjzouozu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sufxvd.cn/gtlrtlsfmr.html

[U49] PHP：只读属性
来源：http://hz.jqgufenzy.top/gtmyubfwtd.html

public readonly string $name
来源：http://hz.aizwys.cn/gtbqxjnoci.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtkxmdpgge.html

public function __construct(private int $id) {}
来源：http://hz.chenzaomai.com/gtrczlysac.html

[U51] PHP：数组解构
来源：http://hz.jqgfzy.top/gtnqiqpxar.html

[$a, $b] = $arr;
来源：http://hz.jqgfzy.top/gtcbncbmte.html

[U52] PHP：箭头函数
来源：http://hz.zhengqikj.top/gtgruwfnwh.html

$double = fn($x) => $x * 2;
来源：http://hz.hnqzz.top/gtzfkblxsx.html

[U53] PHP：空合并运算符
来源：http://hz.yuxming.cn/gtjwqgpttv.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gtenuusave.html

[U54] PHP：空安全调用
来源：http://hz.nwbrower.top/gtbxtkpqmc.html

$obj?->method()
来源：http://hz.nanxuanxn.top/gttjkcleuh.html

[U55] PHP：match 表达式
来源：http://hz.birdmap.top/gtjidrtyck.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sxryk.cn/gteuetatpg.html

[U56] PHP：命名参数
来源：http://hz.jqgufenzy.top/gtkzvlnddx.html

f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtdlrairok.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtdnhshupc.html

"值: {$a}"
来源：http://hz.quarkkingdee.top/gthbzmsjro.html

[U58] PHP：数组三件套
来源：http://hz.havefunace.top/gttidfzxbm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hywenlv.cn/gtgvjiftqe.html

[U59] PHP：自定义排序
来源：http://hz.jinyuanbaomall.cn/gtiurzbdhk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtcjamqrwu.html

[U60] PHP：JSON 编解码
来源：http://hz.ybcxt.top/gtqzlzfbli.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nwbrower.top/gtjjtyjtgz.html

[U61] PHP：正则
来源：http://hz.bjfxy.top/gtvpcwrwrt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtyhcqlcjd.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtpkohbwuq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtbtmjgvui.html

[U63] PHP：文件读写
来源：http://hz.pengpengdd.cyou/gtutvwxort.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cheryme.top/gtaqggggsg.html

[U64] PHP：目录遍历
来源：http://hz.bjfxy.top/gtguksuzgy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.guannengcc.top/gtihxirhih.html

[U65] PHP：会话
来源：http://hz.snrcjt.cn/gtpqasbbbp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.52xcode.cn/gtgauffaaa.html

[U66] PHP：设置 Cookie
来源：http://hz.yanxiufei.cn/gtsasejzvg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhaomingkeji.xyz/gtpsrptzrz.html

[U67] PHP：处理文件上传
来源：http://hz.shangyingyoupin.top/gtlfiedvma.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gteouqeahl.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtrsiprmeg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangshuangyany.cn/gtymwkectv.html

[U69] PHP：PDO 预处理
来源：http://hz.jinghuilouyu.cn/gtqogwsavy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shanyushiyangtech.top/gthixdpjgy.html

[U70] PHP：PDO 事务
来源：http://hz.hnxiangtu.top/gtbspmkiex.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daxiang520.top/gtastvdfqs.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtgazrobpv.html

throw new RuntimeException("失败", 500);
来源：http://hz.hongshengwenyu.top/gtxnmorxdx.html

[U72] PHP：写错误日志
来源：http://hz.yanxiufei.cn/gtsqxsnsqj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.daria6918.cn/gtfcafnluk.html

[U73] PHP：读取 ini 配置
来源：http://hz.tian-w.cn/gtjnyfxorx.html

parse_ini_file("config.ini", true)
来源：http://hz.gotoacloud.top/gtgsimynsc.html

[U74] PHP：读取环境变量
来源：http://hz.9152youxi.cn/gtjlhsnhek.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tianlin.xyz/gtexbumffy.html

[U75] PHP：依赖注入
来源：http://hz.jyoumei.cn/gtohcfdtvz.html

composer require psr/container
来源：http://hz.xuetiantiany.cn/gtncoceuvg.html

[U76] PHP：简单路由
来源：http://hz.yongpay.top/gttfesdkwt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aizwys.cn/gtfcxjnghs.html

[U77] PHP：模板渲染
来源：http://hz.yueranfly.top/gtbcmrfutf.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtlbhaxzpm.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gtthqmnzha.html

composer require --dev phpunit/phpunit
来源：http://hz.xuanzx.com/gtffyxrnej.html

[U79] PHP：静态分析
来源：http://hz.hnqzz.top/gtktubeyxv.html

composer require --dev phpstan/phpstan
来源：http://hz.fengsongda.top/gtafmlenqb.html

[U80] PHP：代码规范修复
来源：http://hz.jinqigufen.top/gtklobwqii.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenjidiqi.icu/gtvahhokgb.html

[U81] JS：初始化项目
来源：http://hz.hysaishi.cn/gtotrsemcj.html

npm init -y;  npm i express
来源：http://hz.xuanzx.com/gtqslzxgyy.html

[U82] JS：package.json 脚本
来源：http://hz.ydjk.org.cn/gtikmvhmyf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.0kj1m.cn/gtxjwhapbw.html

[U83] JS：ES Module 导入导出
来源：http://hz.chenzaomai.com/gtlxgcrbvq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yanxiufei.cn/gteybpoxeq.html

[U84] JS：CommonJS 写法
来源：http://hz.hongshengwenyu.top/gthjnzvgmq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.meibo888.top/gtwndkvhjw.html

[U85] JS：可选链
来源：http://hz.zdqjudy.top/gthhhlgooz.html

a?.b?.c
来源：http://hz.shangyingyoupin.top/gtaehvfpdt.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtjdzgcutn.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtrukryfxs.html

[U87] JS：解构默认值
来源：http://hz.chenjidiqi.icu/gtupoouvpr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hnxiangtu.top/gtcwwhldxs.html

[U88] JS：对象展开合并
来源：http://hz.kuanghao11.cn/gtckjkymrl.html

{ ...a, ...b }
来源：http://hz.nwbrower.top/gtqarzibcu.html

[U89] JS：数组去重
来源：http://hz.ydzc1.top/gtxkluhqhd.html

[...new Set(arr)]
来源：http://hz.meibo888.top/gtyxkmjgaw.html

[U90] JS：数字数组排序
来源：http://hz.hywenlv.cn/gtqatmlekx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtmrfgyrxb.html

[U91] JS：对象键值遍历
来源：http://hz.cheryme.top/gtigncraxu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtesdhyusm.html

[U92] JS：深拷贝
来源：http://hz.cashguo.top/gtmegqorib.html

structuredClone(obj)
来源：http://hz.cqqwz.cn/gtetecaded.html

[U93] JS：模板字符串
来源：http://hz.cqqwz.cn/gtgmafsccz.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gtaedpnszi.html

[U94] JS：箭头函数
来源：http://hz.yongpay.top/gtacruuacs.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtubhnzlxq.html

[U95] JS：Promise 包装
来源：http://hz.chenjidiqi.icu/gtmvlhaoqo.html

new Promise((resolve, reject) => {})
来源：http://hz.aizwys.cn/gtlatbqvvt.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gtaakmekgp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtynbzthsa.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gtarhluwsg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtxvhyokuq.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtpjymgrxz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.52xcode.cn/gtiddjfxti.html

[U99] JS：事件监听
来源：http://hz.zdqjudy.top/gtxqgezmxt.html

el.addEventListener("click", e => {})
来源：http://hz.andypj.xyz/gttrozeegk.html

[U100] JS：DOM 查询
来源：http://hz.aibaodan.cn/gtbedsemvr.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gtmlfuamud.html

[U101] JS：classList 操作
来源：http://hz.shzxlz.cn/gtjmcfkzop.html

el.classList.toggle("active")
来源：http://hz.yonumen.top/gtfbauwpge.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gttuwtnobj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sysykeji.top/gtbafjldhl.html

[U103] JS：定时器
来源：http://hz.chenjidiqi.icu/gtfvbgfdlg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.pengpengdd.cyou/gttxclklwj.html

[U104] JS：防抖
来源：http://hz.ydjk.org.cn/gtnwohezot.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.haohaochexian.top/gtbciiibwt.html

[U105] JS：节流
来源：http://hz.tian-w.cn/gttrnyhwow.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnxiangtu.top/gtanwiqeax.html

[U106] JS：日期格式化
来源：http://hz.sysykeji.top/gtjuduhjel.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cdnleiting.top/gtbvicqorm.html

[U107] JS：数字千分位
来源：http://hz.zhengqikj.top/gtufqescco.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigufen.top/gtlljitxab.html

[U108] JS：随机整数
来源：http://hz.yvedp.cn/gtiknicbjc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.9152youxi.cn/gtfequhpek.html

[U109] JS：数组分组
来源：http://hz.jlsjyb.cn/gtytroafzg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtyhxzpdjk.html

[U110] JS：数组分块
来源：http://hz.zhaomingkeji.xyz/gthofvtcpm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigfzy.top/gtxeevjzdp.html

[U111] JS：对象转 Map
来源：http://hz.mhx1999.top/gtxwjxoptq.html

new Map(Object.entries(obj))
来源：http://hz.jinyuanbaomall.cn/gtbiypmpyc.html

[U112] JS：字符串补位
来源：http://hz.9152youxi.cn/gtsgmqjhlz.html

"7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtxtifmyct.html

[U113] JS：正则替换全部
来源：http://hz.ydjk.org.cn/gtspmwxomg.html

s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtxrhvsydf.html

[U114] JS：JSON 深比较
来源：http://hz.9152youxi.cn/gtsppwukhy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gthawttcot.html

[U115] JS：生成 UUID
来源：http://hz.yj20258.top/gtvlrqpkky.html

crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtvwbltrwz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.redwolf501.top/gtztjabnad.html

/** @param {string} name */ function f(name) {}
来源：http://hz.svipenyu.cn/gtvohllsrc.html

[U117] JS：单元测试
来源：http://hz.ywan-chungtsiang.top/gtefpbcsik.html

npm i -D vitest;  npx vitest
来源：http://hz.jinghuilouyu.cn/gtmgjfszks.html

[U118] JS：开发服务器
来源：http://hz.jinyuanbaomall.cn/gtsdorcnim.html

npm i -D vite;  npx vite
来源：http://hz.yonumen.top/gtoppcpyff.html

[U119] JS：生产构建
来源：http://hz.shangyingyoupin.top/gtlosqkbqp.html

npx vite build
来源：http://hz.52xcode.cn/gtlpkntqlo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhijiandao.cn/gthglyqrmp.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtxfiiztfa.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmxbxkobp.html

统计汇总
来源：http://hz.jinyuanbaomall.cn/gtqqgsxehu.html

================================================================================
来源：http://hz.tianlin.xyz/gtqqpzeagm.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtezlvmbxl.html

Python ......... 252
来源：http://hz.cqqwz.cn/gtlydjmsem.html

PHP ............ 252
来源：http://hz.jlsjyb.cn/gtdahntflz.html

JavaScript ..... 252
来源：http://hz.jiagoushi.top/gtqmagdqmf.html

TypeScript ..... 212
来源：http://hz.hfpthk.cn/gtpbyuxxrx.html

Java ........... 212
来源：http://hz.zhixingplan.top/gtmehxmkdf.html

Go ............. 212
来源：http://hz.jinqigfzy.top/gtcoykcpjz.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtyujjnpmy.html

C# ............. 212
来源：http://hz.gogol.net.cn/gtipgedyov.html

C .............. 30
来源：http://hz.tianlin.xyz/gtpgnslelu.html

C++ ............ 30
来源：http://hz.ivvv.top/gtsxqsgwly.html

SQL ............ 90
来源：http://hz.feifeiyinyue.top/gtabuzunet.html

Bash ........... 80
来源：http://hz.jlsjyb.cn/gtbzpqxzzn.html

Kotlin ......... 15
来源：http://hz.hammf.cn/gtwyujidol.html

Swift .......... 15
来源：http://hz.feifeiyinyue.top/gtrfbrregx.html

Lua ............ 10
来源：http://hz.hnqzz.top/gtacyuahhp.html

Perl ........... 10
来源：http://hz.xuetiantiany.cn/gtqognqbyq.html

Scala .......... 10
来源：http://hz.haohaochexian.top/gtlmpnazkq.html

------------------------------------
来源：http://hz.yvedp.cn/gtugcxlubc.html

合计 ........... 2106 条
来源：http://hz.sufxvd.cn/gtqlupkiky.html

按章节统计：
来源：http://hz.sufxvd.cn/gtgxkcejyk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gtaedyoatj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtycijllfo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtptyhbmrj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtumbkpqiu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenzaomai.com/gtbuqajkem.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtotqiiulm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtjixjzjbb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtdfvpyxud.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtvkocklhp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yueranfly.top/gtpijbovsj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtfropeuhm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtiajyjziw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gttecvdoph.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.fengsongda.top/gthwcjjdwd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuanzx.com/gtbhhhftir.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ehwqpu.com/gtmroawkpy.html

Q SQL 专题                              90
来源：http://hz.hywenlv.cn/gtdqpagfyk.html

R Bash 专题                             80
来源：http://hz.shanyushiyangtech.top/gtutcjobgc.html

S C / C++ 专题                          60
来源：http://hz.feifeiyinyue.top/gtvrxtuqot.html

T 其他语言补充                          60
来源：http://hz.birdmap.top/gtsfdetjlg.html

U 高频实用片段                         120
来源：http://hz.guowangkeji.top/gtwvdnhlkz.html

------------------------------------
来源：http://hz.zhengqikj.top/gtndusrugo.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtgqfeousf.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtinfhkqwi.html

使用提醒
来源：http://hz.shzxlz.cn/gtmdrivxbk.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtddmnvrql.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shzxlz.cn/gtilejmzpa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.tanke756.top/gtrlurekjb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cqqwz.cn/gtidrehioy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.gaohongyu789.top/gtyugbxzkp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.daria6918.cn/gtjhboandk.html

—— 文件结束 ——
来源：http://hz.nanxinkj.top/gtzqaexsoc.html

================================================================================
来源：http://hz.gzhubu.top/gtxfnljbvk.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gtzyhgxswb.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigufen.top/gtdlkqlhcr.html

================================================================================
来源：http://hz.xylfe.cn/gtadfxgyjx.html

【收录内容】
来源：http://hz.cheryme.top/gtamhhbyrc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.andypj.xyz/gtgdtaqpyk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xinyue.icu/gtgdwcarqm.html

SQL · Bash · C · C++
来源：http://hz.dashuyun.cn/gtjvrxsdny.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xinyue.icu/gtldzkbxtl.html

【使用说明】
来源：http://hz.pengpengdd.cyou/gtalhrmqla.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.sysykeji.top/gtffjmvzwr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.wangdashe.top/gtohcjeofg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zycfv.cn/gtwmupnyhi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yonumen.top/gtijuzxkzl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.zhijiandao.cn/gtluvqwgvy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yongpay.top/gtcyxpteyl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cheryme.top/gtxavkdfgp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tian-w.cn/gtyqclxlrj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ywan-chungtsiang.top/gtyjilatvu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.guannengcc.top/gtigjwqome.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinghuilouyu.cn/gtgprfurjs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.havefunace.top/gtgvzepzeg.html

【文件统计】
来源：http://hz.cucudq.cn/gtlqwflmaa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yuanzhike.top/gtilbgrkbr.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gttvzpuece.html

目  录
来源：http://hz.9152youxi.cn/gtublbdurd.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gtdpwsxgnj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtlknkhlnh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtxybmbxkc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtddeomygg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.birdmap.top/gtzunhlytr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sufxvd.cn/gtgbqjgqbw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinyuanbaomall.cn/gtfrvudjkm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtbkwldzps.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtpcpvigjh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtvsbbchgj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.chenjidiqi.icu/gtvfqfuqoq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtuwululfh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtyleboqql.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtoffhpwzj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.wangshuangyany.cn/gteoomyexo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.wangdashe.top/gtxfwjqunr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.sweek.top/gtrwncetwm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gogol.net.cn/gtflmwwnkx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.quarkkingdee.top/gtkdponemt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.52xcode.cn/gtfsdsgafh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtshjdwzem.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtyiwgrtzq.html

================================================================================
来源：http://hz.andypj.xyz/gtewcqlgbp.html

A. 基础语法与类型
来源：http://hz.hysaishi.cn/gtxgwvdbpk.html

================================================================================
来源：http://hz.xziqi.cn/gtqffxzujx.html

[A01] Hello World
来源：http://hz.birdmap.top/gtrqeaqawx.html

Py:   print("Hello, World!")
来源：http://hz.svipenyu.cn/gtjwwshvhm.html

PHP:  echo "Hello, World!";
来源：http://hz.zhoulong.xyz/gtttxsnyis.html

JS:   console.log("Hello, World!");
来源：http://hz.tanke756.top/gtheszoldc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.daria6918.cn/gtfzptzido.html

Java: System.out.println("Hello, World!");
来源：http://hz.nwbrower.top/gtjgdudbdz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yj20258888.top/gtydvvimju.html

Ruby: puts "Hello, World!"
来源：http://hz.0kj1m.cn/gtewgwiwae.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtgoreatyu.html

[A02] 变量声明与赋值
来源：http://hz.kuanghao11.cn/gtphjmtjzu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtmisetjny.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.0kj1m.cn/gtlplkqpnp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenlongwang.top/gtjdpamdvy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yvedp.cn/gtppebvvei.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.wangshuangyany.cn/gtfbcpuyww.html

Go:   name := "Alex"; age := 20
来源：http://hz.vqdsnc.cn/gtlsnpovrl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.sweek.top/gtdbriuzrq.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtizahrefl.html

[A03] 常量定义
来源：http://hz.iojbl.cn/gtgtnnhois.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.chenzaomai.com/gtfmyrurzo.html

PHP:  const PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtgmfknsyw.html

JS:   const PI = 3.14159;
来源：http://hz.nwbrower.top/gtfoenjzfo.html

TS:   const PI: number = 3.14159;
来源：http://hz.dianchejie.cn/gttipayqnh.html

Java: static final double PI = 3.14159;
来源：http://hz.c1oappe.top/gtadvomjze.html

Go:   const PI = 3.14159
来源：http://hz.zycfv.cn/gtplekvbxx.html

Ruby: PI = 3.14159
来源：http://hz.cashguo.top/gthujqawye.html

C#:   const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtqtljyckb.html

[A04] 判断变量类型
来源：http://hz.gaohongyu789.top/gtrsvgjlfu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.hnqzz.top/gtjrbapift.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xylfe.cn/gtbuxuabsm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sweek.top/gtyiwrvvlp.html

TS:   typeof x; x instanceof Date
来源：http://hz.ydzc1.top/gtxaboagqu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinyuanbaomall.cn/gtzdggfnfm.html


<!-- 参考信息 -->