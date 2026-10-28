代发 wailian999

[U43] PHP：声明命名空间
来源：http://hz.feifeiyinyue.top/gtmolilwcj.html

namespace App\Http;
来源：http://hz.ehwqpu.com/gtsrsdwvpb.html

[U44] PHP：开启严格类型
来源：http://hz.havefunace.top/gtjxgpwrvi.html

declare(strict_types=1);
来源：http://hz.316326.xyz/gtvzasjtxx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinqigfzy.top/gtryfjhhgm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtgexfigpk.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtiaxlcgpb.html

?string $name = null
来源：http://hz.yuanzhike.top/gtrablzavu.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gttizzociv.html

int|string $id
来源：http://hz.shuidangran.top/gtztulbaix.html

[U48] PHP：纯枚举
来源：http://hz.shzxlz.cn/gtalasiijg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj202588.top/gtczrsxzxo.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtzahgwgzu.html

public readonly string $name
来源：http://hz.sysykeji.top/gtkdhshoyc.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gthwsfgkpl.html

public function __construct(private int $id) {}
来源：http://hz.dashuyun.cn/gtwryetnsn.html

[U51] PHP：数组解构
来源：http://hz.ywan-chungtsiang.top/gtjffohrds.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtwjdroyec.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gtdhhtgfhx.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtxujrcqop.html

[U53] PHP：空合并运算符
来源：http://hz.jinyuanbaomall.cn/gtlfzqrndh.html

$v = $a ?? $b ?? "default";
来源：http://hz.hfpthk.cn/gtgpmghtmu.html

[U54] PHP：空安全调用
来源：http://hz.sweek.top/gtplnrerix.html

$obj?->method()
来源：http://hz.yj20258.top/gttesndrfp.html

[U55] PHP：match 表达式
来源：http://hz.meibo888.top/gtqmkycuuq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yvedp.cn/gtsjjbxkzk.html

[U56] PHP：命名参数
来源：http://hz.zhixingplan.top/gtlsxwbvyk.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtailzbjlc.html

[U57] PHP：字符串插值
来源：http://hz.sufxvd.cn/gtiapfmstw.html

"值: {$a}"
来源：http://hz.hongshengwenyu.top/gtepuhuvnk.html

[U58] PHP：数组三件套
来源：http://hz.xuanzx.com/gtvyghmejf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ywan-chungtsiang.top/gthgwhfsxl.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtbvcuwcnl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtavjftdpf.html

[U60] PHP：JSON 编解码
来源：http://hz.yongpay.top/gtrcehsnwt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.nanxinkj.top/gtoxckbpjv.html

[U61] PHP：正则
来源：http://hz.cucudq.cn/gtpoulydgv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtwilhwowa.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtlyogheqe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangshuangyany.cn/gtpryzaahh.html

[U63] PHP：文件读写
来源：http://hz.gogol.net.cn/gtfeavervl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangkeji.top/gtxyvsxyhs.html

[U64] PHP：目录遍历
来源：http://hz.ydjk.org.cn/gtcbgbruom.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gtwxzczmtf.html

[U65] PHP：会话
来源：http://hz.daxiang520.top/gtmqoivjgx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinqigfzy.top/gtlimssjym.html

[U66] PHP：设置 Cookie
来源：http://hz.jinghuilouyu.cn/gtdlknjabk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtgjagajjg.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtkdcejhuw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ydjk.org.cn/gtyqhaytcb.html

[U68] PHP：PDO 连接
来源：http://hz.shangyingyoupin.top/gtjpnssazy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ehwqpu.com/gtyiqfyodr.html

[U69] PHP：PDO 预处理
来源：http://hz.ivvv.top/gtifebidxr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gogol.net.cn/gtxudkfamx.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtyojnltko.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.birdmap.top/gtzziqkgqx.html

[U71] PHP：抛出异常
来源：http://hz.316326.xyz/gtkzoflwmb.html

throw new RuntimeException("失败", 500);
来源：http://hz.daxiang520.top/gtauyynrmb.html

[U72] PHP：写错误日志
来源：http://hz.zhiwuduotai.top/gtufsvlmiv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.vqdsnc.cn/gtbulmroey.html

[U73] PHP：读取 ini 配置
来源：http://hz.aibaodan.cn/gtecbzwehh.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258888.top/gttshqofat.html

[U74] PHP：读取环境变量
来源：http://hz.yj20258888.top/gtzenxxtjr.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sysykeji.top/gtayaxziwa.html

[U75] PHP：依赖注入
来源：http://hz.ydzc1.top/gtegtqegfb.html

composer require psr/container
来源：http://hz.tianlin.xyz/gtbgdlthza.html

[U76] PHP：简单路由
来源：http://hz.zycfv.cn/gtxwmfzfqg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtqifncrpl.html

[U77] PHP：模板渲染
来源：http://hz.yanxiufei.cn/gtlfxakpdj.html

composer require twig/twig
来源：http://hz.jyoumei.cn/gtnkbsgaws.html

[U78] PHP：单元测试
来源：http://hz.xuanzx.com/gtlyyuhumi.html

composer require --dev phpunit/phpunit
来源：http://hz.yanxiufei.cn/gtlszyhkby.html

[U79] PHP：静态分析
来源：http://hz.tanke756.top/gtbsgzohrx.html

composer require --dev phpstan/phpstan
来源：http://hz.dashuyun.cn/gtlunyurca.html

[U80] PHP：代码规范修复
来源：http://hz.tian-w.cn/gtasqkswzv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.chenjidiqi.icu/gtdolejfkt.html

[U81] JS：初始化项目
来源：http://hz.yvedp.cn/gtnuhhhjmk.html

npm init -y;  npm i express
来源：http://hz.jinyuanbaomall.cn/gtsxewzitn.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtbjqlbcme.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nanxuanxn.top/gtjmmajymk.html

[U83] JS：ES Module 导入导出
来源：http://hz.gzhubu.top/gtaebrvsmk.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.vqdsnc.cn/gtsygcppfg.html

[U84] JS：CommonJS 写法
来源：http://hz.cqqwz.cn/gtgywrqfbx.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangdashe.top/gtdoufjjmg.html

[U85] JS：可选链
来源：http://hz.shzxlz.cn/gtknqypzen.html

a?.b?.c
来源：http://hz.xziqi.cn/gtzcxsepyy.html

[U86] JS：空值合并
来源：http://hz.tanke756.top/gttfgwwsji.html

a ?? b
来源：http://hz.guowangkeji.top/gtkrikykjo.html

[U87] JS：解构默认值
来源：http://hz.cucudq.cn/gtffejzpbf.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtodapofca.html

[U88] JS：对象展开合并
来源：http://hz.ppjwa.cn/gtycqsjzes.html

{ ...a, ...b }
来源：http://hz.daria6918.cn/gttapmxzkg.html

[U89] JS：数组去重
来源：http://hz.zhaomingkeji.xyz/gtjaflacsi.html

[...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtvjtwghbb.html

[U90] JS：数字数组排序
来源：http://hz.haohaochexian.top/gtyphjcuvf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtzajuyspb.html

[U91] JS：对象键值遍历
来源：http://hz.wangdashe.top/gtczdihpjl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cdnleiting.top/gtfirdymnr.html

[U92] JS：深拷贝
来源：http://hz.zhixingplan.top/gtgwyavpwc.html

structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtedfvpmas.html

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtzgmmsyqg.html

`共 ${n} 条`
来源：http://hz.shuidangran.top/gtblpmnegp.html

[U94] JS：箭头函数
来源：http://hz.guannengcc.top/gtukdqoakk.html

const double = x => x * 2;
来源：http://hz.0kj1m.cn/gtdqhvtbth.html

[U95] JS：Promise 包装
来源：http://hz.xziqi.cn/gtcdyokxfv.html

new Promise((resolve, reject) => {})
来源：http://hz.chenlongwang.top/gtnhjrsdof.html

[U96] JS：async/await 与异常
来源：http://hz.hammf.cn/gtjqcszqhz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtgwxfnfqe.html

[U97] JS：并发请求
来源：http://hz.guannengcc.top/gtflqawprj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtxoejhsnn.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinghuilouyu.cn/gtswgzgfev.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.c1oappe.top/gtcdyndxyl.html

[U99] JS：事件监听
来源：http://hz.yonumen.top/gtvcziudog.html

el.addEventListener("click", e => {})
来源：http://hz.hywenlv.cn/gtxwzihbkl.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtqqmefruj.html

document.querySelector(".item")
来源：http://hz.tian-w.cn/gtoeaculps.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gtbucjzsjl.html

el.classList.toggle("active")
来源：http://hz.chenzaomai.com/gtrkvuykvd.html

[U102] JS：本地存储
来源：http://hz.yvedp.cn/gthtbbnjjb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhoulong.xyz/gtpyvddipr.html

[U103] JS：定时器
来源：http://hz.feifeiyinyue.top/gtvnujceht.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cashguo.top/gthlbwmvfm.html

[U104] JS：防抖
来源：http://hz.dashuyun.cn/gtwwsvbspx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenlongwang.top/gtopxnitut.html

[U105] JS：节流
来源：http://hz.yvedp.cn/gtlziqqdfm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.smart0.xyz/gtwwxuqttu.html

[U106] JS：日期格式化
来源：http://hz.yj20258888.top/gtimfvglvx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tanke756.top/gtqbbamnkk.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gtxccnoatr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hongshengwenyu.top/gtuudjxgbl.html

[U108] JS：随机整数
来源：http://hz.xingfuxueyuan.xyz/gtdqkcfcsa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.smart0.xyz/gtxzlmextb.html

[U109] JS：数组分组
来源：http://hz.0kj1m.cn/gtmlqgcnyj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtxlijvacn.html

[U110] JS：数组分块
来源：http://hz.316326.xyz/gtlhlmctdm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sxryk.cn/gtynnquaxv.html

[U111] JS：对象转 Map
来源：http://hz.xuetiantiany.cn/gtwhqqjzra.html

new Map(Object.entries(obj))
来源：http://hz.andypj.xyz/gthhevhrds.html

[U112] JS：字符串补位
来源：http://hz.feifeiyinyue.top/gtcqhuhcew.html

"7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtxxjcffzx.html

[U113] JS：正则替换全部
来源：http://hz.snrcjt.cn/gtomcqziyc.html

s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtsbcudswl.html

[U114] JS：JSON 深比较
来源：http://hz.ppjwa.cn/gtsytrdzgz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtecgnhpwy.html

[U115] JS：生成 UUID
来源：http://hz.316326.xyz/gtzcdafxct.html

crypto.randomUUID()
来源：http://hz.aizwys.cn/gtsfetgxwh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.daxiang520.top/gthlvkkiit.html

/** @param {string} name */ function f(name) {}
来源：http://hz.feifeiyinyue.top/gtgsutfcrl.html

[U117] JS：单元测试
来源：http://hz.hongshengwenyu.top/gtgnchobtl.html

npm i -D vitest;  npx vitest
来源：http://hz.quarkkingdee.top/gtgxamzchl.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtfljzbmbq.html

npm i -D vite;  npx vite
来源：http://hz.ivvv.top/gtqonhazhn.html

[U119] JS：生产构建
来源：http://hz.hysaishi.cn/gtlohkryhq.html

npx vite build
来源：http://hz.cashguo.top/gtkageyhbi.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.0kj1m.cn/gthpyxgybj.html

import.meta.env.VITE_API_URL
来源：http://hz.jianghu66.top/gtwgwanokr.html

================================================================================
来源：http://hz.hywenlv.cn/gtkopvwgdv.html

统计汇总
来源：http://hz.ppjwa.cn/gtkvcjrqgm.html

================================================================================
来源：http://hz.tanke756.top/gtzufbmqsn.html

按语言统计（条）：
来源：http://hz.fzhhl.top/gtawrmnmgo.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtzqpigart.html

PHP ............ 252
来源：http://hz.iojbl.cn/gtqssgvyom.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gttlluxdqp.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gtylbafofe.html

Java ........... 212
来源：http://hz.aizwys.cn/gtzpjejevc.html

Go ............. 212
来源：http://hz.yonumen.top/gtnyimmpoa.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtcvjxnpbn.html

C# ............. 212
来源：http://hz.chenzaomai.com/gtvhuvrvkj.html

C .............. 30
来源：http://hz.ybcxt.top/gtygklyvre.html

C++ ............ 30
来源：http://hz.jinghuilouyu.cn/gtaqcwcttl.html

SQL ............ 90
来源：http://hz.shanyushiyangkeji.top/gtajudgpez.html

Bash ........... 80
来源：http://hz.ydjk.org.cn/gtxaeepoif.html

Kotlin ......... 15
来源：http://hz.vqdsnc.cn/gtouychqtd.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtuaxvdbye.html

Lua ............ 10
来源：http://hz.zhongyouzk.top/gtdrsrszld.html

Perl ........... 10
来源：http://hz.jyoumei.cn/gtrdbqaxsx.html

Scala .......... 10
来源：http://hz.ywan-chungtsiang.top/gtlifoemrh.html

------------------------------------
来源：http://hz.jyoumei.cn/gtvipybjaz.html

合计 ........... 2106 条
来源：http://hz.0kj1m.cn/gtgxjrloah.html

按章节统计：
来源：http://hz.hysaishi.cn/gtjpyzspkj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ydjk.org.cn/gtegcndhnt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtvzflsucu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtcwuckcrh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtxtgezrgw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hysaishi.cn/gtqhjonizi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gtjvgxfgsv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtvfsicjnw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hysaishi.cn/gtdikqlmzx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtcbqhjvzv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.birdmap.top/gtjppzhnja.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtpdehxwqq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtyaniqhiz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtejsswsdg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.feifeiyinyue.top/gtceyedfwv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.haohaochexian.top/gtmklukwah.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtsnwoziab.html

Q SQL 专题                              90
来源：http://hz.yuxming.cn/gtywhpmgxl.html

R Bash 专题                             80
来源：http://hz.ivvv.top/gtwwbdwvng.html

S C / C++ 专题                          60
来源：http://hz.dianchejie.cn/gtfiuqikvr.html

T 其他语言补充                          60
来源：http://hz.zdqjudy.top/gtpdobzcvi.html

U 高频实用片段                         120
来源：http://hz.ivvv.top/gtuuzyhdde.html

------------------------------------
来源：http://hz.hysaishi.cn/gtdjndrzbs.html

合计                                  2106 条
来源：http://hz.shzxlz.cn/gtqjnggwla.html

--------------------------------------------------------------------------------
来源：http://hz.yonumen.top/gtkvxukztx.html

使用提醒
来源：http://hz.chenjidiqi.icu/gtyukvhgvb.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtospvpybz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gotoacloud.top/gtscxwztny.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jianghu66.top/gtaeunegzq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jlsjyb.cn/gtdwjijnsy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtcyheofwg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yanxiufei.cn/gtizbtcpxz.html

—— 文件结束 ——
来源：http://hz.xylfe.cn/gtyzgeyffo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwfpmwksw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jyoumei.cn/gtdyjcrnse.html

Common Programming Examples Cheat Book
来源：http://hz.gaohongyu789.top/gtihhwqntw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtaushoxgq.html

【收录内容】
来源：http://hz.redwolf501.top/gtrhowfevf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zhongyouzk.top/gtmtfjzdgr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhengqikj.top/gtrtstmhft.html

SQL · Bash · C · C++
来源：http://hz.gogol.net.cn/gtdmomdcea.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinyuanbaomall.cn/gtxyajwkyz.html

【使用说明】
来源：http://hz.shuidangran.top/gtpobslrdq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhijiandao.cn/gtysjxrwvl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hfpthk.cn/gtsfsieoou.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.iojbl.cn/gtrcnppwxk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dianchejie.cn/gtwyubfaus.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxuanxn.top/gtxaqxrlzq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yonumen.top/gtnvunvzpj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.iojbl.cn/gtqovvplrh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhiwuduotai.top/gtdxmewowa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.bjfxy.top/gthcxdsmln.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tanke756.top/gtvxhpkvdu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yonumen.top/gtfaiwzklj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.kuanghao11.cn/gtvitfozoy.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtccisxmex.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.svipenyu.cn/gtuzolaobr.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtnmhvgilj.html

目  录
来源：http://hz.ydjk.org.cn/gtcwsausco.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtzxoxcxjn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gtldghibzv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtswfbqedt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtrnludvgg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daria6918.cn/gtkigxfery.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.wangshuangyany.cn/gtldspqeih.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtbmgrcyoz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.sxryk.cn/gtvrkiytmc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.shanyushiyangtech.top/gthinfkhtr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.pycfn.com/gtwejhlpts.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.redwolf501.top/gtbmidmscg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtrcidwiby.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jqgfzy.top/gtmevhzzym.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ywan-chungtsiang.top/gtfmfztwzy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtbubssqzd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zdqjudy.top/gtepanpwco.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtklriiygh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.guannengcc.top/gtdpjgpvrr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhijiandao.cn/gtrlzxddno.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxinkj.top/gtkdkwxtfq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gtswhcnjpj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gzhubu.top/gtjlhsxhdd.html

================================================================================
来源：http://hz.shzxlz.cn/gtmjtggtyb.html

A. 基础语法与类型
来源：http://hz.xuetiantiany.cn/gtpsandtkp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtphojdcpp.html

[A01] Hello World
来源：http://hz.tian-w.cn/gtocjkgvbl.html

Py:   print("Hello, World!")
来源：http://hz.havefunace.top/gtblpvmohm.html

PHP:  echo "Hello, World!";
来源：http://hz.ydjk.org.cn/gtfooebtyu.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtczdegedv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.316326.xyz/gtwldhiqtv.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhixingplan.top/gtvcieiaeq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yvedp.cn/gtnonzboip.html

Ruby: puts "Hello, World!"
来源：http://hz.shanyushiyangkeji.top/gtapivjcqy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.daxiang520.top/gtcruhnmed.html

[A02] 变量声明与赋值
来源：http://hz.gzhubu.top/gtktaulobr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.guannengcc.top/gtchjifrxx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jianghu66.top/gtcxgxgxxm.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.wangshuangyany.cn/gtempfrkqn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.nanxinkj.top/gtqavwzkwp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtbzcogemo.html

Go:   name := "Alex"; age := 20
来源：http://hz.hammf.cn/gtnfcpjfia.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hywenlv.cn/gtfbuxdofm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.daxiang520.top/gtfumaxrgk.html

[A03] 常量定义
来源：http://hz.zhengqikj.top/gtuhsebirh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sweek.top/gtovyxvlmk.html

PHP:  const PI = 3.14159;
来源：http://hz.guowangkeji.top/gtumviqppo.html

JS:   const PI = 3.14159;
来源：http://hz.yuxming.cn/gtgxigvgfa.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuanzhike.top/gtrayglyqr.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtvwzkawuo.html

Go:   const PI = 3.14159
来源：http://hz.ywan-chungtsiang.top/gtugntsyrv.html

Ruby: PI = 3.14159
来源：http://hz.vqdsnc.cn/gtpsshwjqh.html

C#:   const double PI = 3.14159;
来源：http://hz.gogol.net.cn/gtyrdsirfx.html

[A04] 判断变量类型
来源：http://hz.gzhubu.top/gtisvtlxch.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.snrcjt.cn/gtunaavaef.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.vqdsnc.cn/gtmsdbkhoa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xinyue.icu/gtqktjmbik.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gtgcjgghav.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shzxlz.cn/gtcqsmubhm.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.wangshuangyany.cn/gtdlcnrcrm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cdnleiting.top/gtgazsurgn.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhongyouzk.top/gtnxfllipn.html

[A05] 整数除法与取模
来源：http://hz.wangshuangyany.cn/gtqjejakjf.html


<!-- 参考信息 -->