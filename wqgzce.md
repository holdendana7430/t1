代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtjpltpfud.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtouxuiaqx.html

[U46] PHP：可空类型
来源：http://hz.vqdsnc.cn/gtyttonwmu.html

?string $name = null
来源：http://hz.dashuyun.cn/gtowhtvkpw.html

[U47] PHP：联合类型
来源：http://hz.zhengqikj.top/gtuucbbnuk.html

int|string $id
来源：http://hz.shangyingyoupin.top/gtywoazhsl.html

[U48] PHP：纯枚举
来源：http://hz.shzxlz.cn/gtpsynkyco.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dashuyun.cn/gtlmrbkdiv.html

[U49] PHP：只读属性
来源：http://hz.jiagoushi.top/gtpdwxmxic.html

public readonly string $name
来源：http://hz.guowangkeji.top/gtxbalbfvz.html

[U50] PHP：构造器属性提升
来源：http://hz.quarkkingdee.top/gtmnwtfgsn.html

public function __construct(private int $id) {}
来源：http://hz.xingfuxueyuan.xyz/gtcthxxbca.html

[U51] PHP：数组解构
来源：http://hz.0kj1m.cn/gtvbmnuvtv.html

[$a, $b] = $arr;
来源：http://hz.dashuyun.cn/gtofericbs.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtwwfyuslu.html

$double = fn($x) => $x * 2;
来源：http://hz.zhoulong.xyz/gtcqvmvxwz.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtwatnaujl.html

$v = $a ?? $b ?? "default";
来源：http://hz.xziqi.cn/gtvenzvdbg.html

[U54] PHP：空安全调用
来源：http://hz.xylfe.cn/gtgofkboke.html

$obj?->method()
来源：http://hz.yj20258.top/gtrjgfduob.html

[U55] PHP：match 表达式
来源：http://hz.ivvv.top/gtmroupnbe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gtbbfupmjf.html

[U56] PHP：命名参数
来源：http://hz.pengpengdd.cyou/gtpaedbolm.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtreybfbku.html

[U57] PHP：字符串插值
来源：http://hz.sweek.top/gtwwzmmypi.html

"值: {$a}"
来源：http://hz.0kj1m.cn/gtjylihfqt.html

[U58] PHP：数组三件套
来源：http://hz.quarkkingdee.top/gtmwfgbnde.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.dashuyun.cn/gtmncqepef.html

[U59] PHP：自定义排序
来源：http://hz.xingfuxueyuan.xyz/gtjtpkiusf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtoaywysxy.html

[U60] PHP：JSON 编解码
来源：http://hz.gaohongyu789.top/gtnmmrhpon.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.0kj1m.cn/gtffeyznnw.html

[U61] PHP：正则
来源：http://hz.chenzaomai.com/gtttifmxoy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtbbiqwodr.html

[U62] PHP：日期对象
来源：http://hz.gaohongyu789.top/gtpvjvgeuo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gtdyxngmbn.html

[U63] PHP：文件读写
来源：http://hz.zhiwuduotai.top/gtuygnyrve.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangshuangyany.cn/gtggjicoau.html

[U64] PHP：目录遍历
来源：http://hz.ydzc1.top/gtzupfhzxy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shangyingyoupin.top/gtsdublggy.html

[U65] PHP：会话
来源：http://hz.sysykeji.top/gtyednamch.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtwesrqwfl.html

[U66] PHP：设置 Cookie
来源：http://hz.zhijiandao.cn/gtmejgrrqm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.0kj1m.cn/gtznrvrcnm.html

[U67] PHP：处理文件上传
来源：http://hz.xuetiantiany.cn/gtybvwyofu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yangfankeji.com/gtqpionvij.html

[U68] PHP：PDO 连接
来源：http://hz.yuanzhike.top/gtupqviizp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtslynbzxf.html

[U69] PHP：PDO 预处理
来源：http://hz.ydjk.org.cn/gtgbzgupxe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.pycfn.com/gtkrcdhney.html

[U70] PHP：PDO 事务
来源：http://hz.aibaodan.cn/gtukckgjix.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtclcakgbg.html

[U71] PHP：抛出异常
来源：http://hz.yuxming.cn/gtdxsclgjy.html

throw new RuntimeException("失败", 500);
来源：http://hz.svipenyu.cn/gtpdslkbgy.html

[U72] PHP：写错误日志
来源：http://hz.0kj1m.cn/gtqzyewcju.html

error_log("失败: " . $e->getMessage());
来源：http://hz.gogol.net.cn/gtqhgjzcne.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuxming.cn/gtakyezsqs.html

parse_ini_file("config.ini", true)
来源：http://hz.dashuyun.cn/gtfdgfqalj.html

[U74] PHP：读取环境变量
来源：http://hz.dashuyun.cn/gtynzqizgu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.guowangkeji.top/gtzjzqkvlr.html

[U75] PHP：依赖注入
来源：http://hz.zhoulong.xyz/gtovudwcga.html

composer require psr/container
来源：http://hz.guowangkeji.top/gtmrsykdcm.html

[U76] PHP：简单路由
来源：http://hz.svipenyu.cn/gtouspuodc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtasmnfbyn.html

[U77] PHP：模板渲染
来源：http://hz.quarkkingdee.top/gtsppykpdl.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtvvtlxueg.html

[U78] PHP：单元测试
来源：http://hz.snrcjt.cn/gtoosjwwsr.html

composer require --dev phpunit/phpunit
来源：http://hz.jyoumei.cn/gtwvaxuuxx.html

[U79] PHP：静态分析
来源：http://hz.xinyue.icu/gtgfpgbzhg.html

composer require --dev phpstan/phpstan
来源：http://hz.zhixingplan.top/gtjunsbehj.html

[U80] PHP：代码规范修复
来源：http://hz.wangshuangyany.cn/gtxfvjpzsm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.tanke756.top/gtpgvstmoi.html

[U81] JS：初始化项目
来源：http://hz.zdqjudy.top/gtmdtjxnhz.html

npm init -y;  npm i express
来源：http://hz.wangdashe.top/gtdntvmnry.html

[U82] JS：package.json 脚本
来源：http://hz.yvedp.cn/gtrdgdcqpf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhijiandao.cn/gtwspxmxer.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhijiandao.cn/gtxzsqyeac.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yonumen.top/gtcxihtmrt.html

[U84] JS：CommonJS 写法
来源：http://hz.aibaodan.cn/gtfmcilggb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yanxiufei.cn/gttqqniodu.html

[U85] JS：可选链
来源：http://hz.316326.xyz/gtffvijbne.html

a?.b?.c
来源：http://hz.yj20258888.top/gtbqlmmvxr.html

[U86] JS：空值合并
来源：http://hz.yangfankeji.com/gtmnovwrgh.html

a ?? b
来源：http://hz.zhixingplan.top/gtcqgwofaj.html

[U87] JS：解构默认值
来源：http://hz.birdmap.top/gtdjyhknrx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.ivvv.top/gttibhjyjx.html

[U88] JS：对象展开合并
来源：http://hz.jinyuanbaomall.cn/gttliocqxp.html

{ ...a, ...b }
来源：http://hz.fzhhl.top/gtfvnzvuvg.html

[U89] JS：数组去重
来源：http://hz.ivvv.top/gtdbqczapf.html

[...new Set(arr)]
来源：http://hz.jiagoushi.top/gtfuoynzdk.html

[U90] JS：数字数组排序
来源：http://hz.birdmap.top/gtacmjjbmd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtdggwcllc.html

[U91] JS：对象键值遍历
来源：http://hz.xylfe.cn/gtfbyoyifs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cheryme.top/gtiqrcuvnc.html

[U92] JS：深拷贝
来源：http://hz.ydjk.org.cn/gtraaowgaw.html

structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtwgwbsvlh.html

[U93] JS：模板字符串
来源：http://hz.kuanghao11.cn/gtzgtwlugb.html

`共 ${n} 条`
来源：http://hz.jinqigfzy.top/gtttlamvfo.html

[U94] JS：箭头函数
来源：http://hz.meibo888.top/gttzetsxyo.html

const double = x => x * 2;
来源：http://hz.meibo888.top/gtvfrigyhp.html

[U95] JS：Promise 包装
来源：http://hz.yueranfly.top/gtlggpptvt.html

new Promise((resolve, reject) => {})
来源：http://hz.cqqwz.cn/gtcjfsjfsb.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtyvcsogtr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtpstwyxdp.html

[U97] JS：并发请求
来源：http://hz.aibaodan.cn/gteuodghte.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtjrmlnxzn.html

[U98] JS：fetch 带 JSON
来源：http://hz.hongshengwenyu.top/gtmpqvlxas.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.havefunace.top/gtkbepwtag.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtcfhafnbq.html

el.addEventListener("click", e => {})
来源：http://hz.haohaochexian.top/gtcfnpbwtc.html

[U100] JS：DOM 查询
来源：http://hz.jyoumei.cn/gtwiimrsbi.html

document.querySelector(".item")
来源：http://hz.yueranfly.top/gtefwtbfky.html

[U101] JS：classList 操作
来源：http://hz.cqqwz.cn/gtqiestfba.html

el.classList.toggle("active")
来源：http://hz.zhongyouzk.top/gtwafjtraa.html

[U102] JS：本地存储
来源：http://hz.0kj1m.cn/gtwqfjwfhj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhijiandao.cn/gtgfnozoeb.html

[U103] JS：定时器
来源：http://hz.ydjk.org.cn/gtnbdeqtvm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtfolbodph.html

[U104] JS：防抖
来源：http://hz.shanyushiyangtech.top/gtgpvfzqmg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtybyruqsz.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtgakgcecz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.vqdsnc.cn/gttdcwtbbx.html

[U106] JS：日期格式化
来源：http://hz.hongshengwenyu.top/gtmadqstyf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cashguo.top/gtizalnabj.html

[U107] JS：数字千分位
来源：http://hz.daria6918.cn/gtborjpifx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtsywcjygc.html

[U108] JS：随机整数
来源：http://hz.yanxiufei.cn/gtpgdcfqiu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.snrcjt.cn/gtlwsrkzas.html

[U109] JS：数组分组
来源：http://hz.yueranfly.top/gtmsuxoxgc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtwkzpfrnd.html

[U110] JS：数组分块
来源：http://hz.yueranfly.top/gtbitrwtzm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yanxiufei.cn/gtiqhakcmn.html

[U111] JS：对象转 Map
来源：http://hz.fengsongda.top/gtvqhhjwgh.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gthzggpebv.html

[U112] JS：字符串补位
来源：http://hz.cucudq.cn/gtfialsuib.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtrspjdvks.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtthfjuauy.html

s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtxeseqgmi.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigufen.top/gtmuilivyb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtizejbxdl.html

[U115] JS：生成 UUID
来源：http://hz.smart0.xyz/gtxvkuimpq.html

crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtvwcrmgfw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hnxiangtu.top/gtswabqcfo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj202588.top/gtkzrcpxhn.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtieuofqbx.html

npm i -D vitest;  npx vitest
来源：http://hz.hfpthk.cn/gtmxddaobj.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gtwhubrqlc.html

npm i -D vite;  npx vite
来源：http://hz.yuxming.cn/gtjmvtbgyj.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gtoylrotmm.html

npx vite build
来源：http://hz.nanxuanxn.top/gtvjqemeju.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sufxvd.cn/gtfhgieqer.html

import.meta.env.VITE_API_URL
来源：http://hz.shanyushiyangtech.top/gtotrcbckz.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgozceixp.html

统计汇总
来源：http://hz.yueranfly.top/gtmfirflwf.html

================================================================================
来源：http://hz.mhx1999.top/gtkaaewbod.html

按语言统计（条）：
来源：http://hz.quarkkingdee.top/gtbiaymhut.html

Python ......... 252
来源：http://hz.zhoulong.xyz/gtysfrdwoa.html

PHP ............ 252
来源：http://hz.tian-w.cn/gtfysepsne.html

JavaScript ..... 252
来源：http://hz.daxiang520.top/gtiwanjyhw.html

TypeScript ..... 212
来源：http://hz.yangfankeji.com/gtnymcocsx.html

Java ........... 212
来源：http://hz.c1oappe.top/gtnlersosh.html

Go ............. 212
来源：http://hz.meibo888.top/gtuturxndt.html

Ruby ........... 212
来源：http://hz.c1oappe.top/gtosgllvjx.html

C# ............. 212
来源：http://hz.daria6918.cn/gtleimreog.html

C .............. 30
来源：http://hz.vqdsnc.cn/gtcjictigr.html

C++ ............ 30
来源：http://hz.pycfn.com/gtqryhnzdj.html

SQL ............ 90
来源：http://hz.pengpengdd.cyou/gtozeedjex.html

Bash ........... 80
来源：http://hz.hongshengwenyu.top/gtyuehdvnj.html

Kotlin ......... 15
来源：http://hz.yj20258888.top/gtasrwmglj.html

Swift .......... 15
来源：http://hz.xinyue.icu/gtdcixysji.html

Lua ............ 10
来源：http://hz.jlsjyb.cn/gtgiqshzrx.html

Perl ........... 10
来源：http://hz.iojbl.cn/gtgxqziilz.html

Scala .......... 10
来源：http://hz.zdqjudy.top/gtqgzruzyj.html

------------------------------------
来源：http://hz.zhixingplan.top/gtxuckvwib.html

合计 ........... 2106 条
来源：http://hz.shangyingyoupin.top/gtkfaoewzv.html

按章节统计：
来源：http://hz.xuanzx.com/gtmdesweth.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtnorgfzth.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtixokrwvi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtuthnqqma.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jinqigufen.top/gtmuritnie.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.daxiang520.top/gtozkgrrbw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtcloqxnkp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtvntuhnud.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gtijrxpwra.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtvkbqfixi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gzhubu.top/gtjalqhnps.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtzferonmk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtkvesmlvy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtqtlhpqlw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtjkgdgpju.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhengqikj.top/gtosaqvcqs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtwlsvuumb.html

Q SQL 专题                              90
来源：http://hz.c1oappe.top/gtcemqxlnr.html

R Bash 专题                             80
来源：http://hz.dashuyun.cn/gtcwiappqz.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtzaijbipi.html

T 其他语言补充                          60
来源：http://hz.zycfv.cn/gtkkkqgfpm.html

U 高频实用片段                         120
来源：http://hz.tanke756.top/gtyyqkpbvw.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtnqsfokgf.html

合计                                  2106 条
来源：http://hz.havefunace.top/gtfmyopypu.html

--------------------------------------------------------------------------------
来源：http://hz.andypj.xyz/gtvkoplepq.html

使用提醒
来源：http://hz.mhx1999.top/gtwdbxaqdn.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtjtnzxhqr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hywenlv.cn/gttevsrbgm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xziqi.cn/gtsevalmeb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnxiangtu.top/gtezqacwbt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhixingplan.top/gtjiueisje.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cheryme.top/gtdjjzseeu.html

—— 文件结束 ——
来源：http://hz.gogol.net.cn/gtexrfcwtl.html

================================================================================
来源：http://hz.zhixingplan.top/gthwvwoowa.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jqgfzy.top/gtvrgygatu.html

Common Programming Examples Cheat Book
来源：http://hz.pycfn.com/gtyelhwaso.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxlkikaev.html

【收录内容】
来源：http://hz.zhaomingkeji.xyz/gtvnznrjvf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tanke756.top/gtxnfzinal.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ybcxt.top/gtapmgskos.html

SQL · Bash · C · C++
来源：http://hz.haohaochexian.top/gtiaoavqfb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ivvv.top/gtjgtwkoqt.html

【使用说明】
来源：http://hz.xuetiantiany.cn/gtleercpsw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.smart0.xyz/gtgbzyjwtm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nanxinkj.top/gtyuxvvkwg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zycfv.cn/gtvxxkaspy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.9152youxi.cn/gtbpvlwdnd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yonumen.top/gtyyojnwwq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tian-w.cn/gtfuhmxanz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.sysykeji.top/gtxbtewqmj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigfzy.top/gtrxlmrnpm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuanzhike.top/gtizdwpueh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhixingplan.top/gtbqoloehg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinqigufen.top/gtxlkspubt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tian-w.cn/gtgkwhozlf.html

【文件统计】
来源：http://hz.xylfe.cn/gtmujpukwx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.chenlongwang.top/gtlmrhkgfd.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtvbczawtd.html

目  录
来源：http://hz.wangdashe.top/gtdchdilmg.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigfzy.top/gttmflljai.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtooevhebf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.9152youxi.cn/gtwoiksfle.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtepzixole.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.shangyingyoupin.top/gtbouxbdra.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yj202588.top/gtpvdrtasw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.aibaodan.cn/gtlmqcdeqy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtuywypjpo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhaomingkeji.xyz/gtewgkfpkp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtnzolskzp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.nanxuanxn.top/gtpnrigzol.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtxgrekdqg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtvyidwszl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtpvkumaic.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtqykqlouy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinqigufen.top/gtkogbmdrg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gthpibpekp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nwbrower.top/gttfxtnwhl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhaomingkeji.xyz/gtgghnjdel.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gaohongyu789.top/gtqzwhibaq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtrphnejlq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtyhxnrdnj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtvqkkflry.html

A. 基础语法与类型
来源：http://hz.smart0.xyz/gtbzgtlart.html

================================================================================
来源：http://hz.cdnleiting.top/gtvtlsrkfp.html

[A01] Hello World
来源：http://hz.nwbrower.top/gtrgjoehpz.html

Py:   print("Hello, World!")
来源：http://hz.svipenyu.cn/gtiqizhknd.html

PHP:  echo "Hello, World!";
来源：http://hz.shanyushiyangkeji.top/gtungdyuko.html

JS:   console.log("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtntceaqco.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj20258888.top/gtedsngtwp.html

Java: System.out.println("Hello, World!");
来源：http://hz.shanyushiyangkeji.top/gtahpdqxlz.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sysykeji.top/gtosabpkpz.html

Ruby: puts "Hello, World!"
来源：http://hz.gzhubu.top/gtevhunmlg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydzc1.top/gtvgraqajf.html

[A02] 变量声明与赋值
来源：http://hz.feifeiyinyue.top/gtgbugwult.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.havefunace.top/gthwqomxqv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zhoulong.xyz/gtlcdgeomh.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ydjk.org.cn/gtfaxwvcjl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cucudq.cn/gtywlesvxy.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtzbtlgvlk.html

Go:   name := "Alex"; age := 20
来源：http://hz.shanyushiyangtech.top/gtxqhwmrgm.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gogol.net.cn/gtcdevyqhv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtlrogguvw.html

[A03] 常量定义
来源：http://hz.yj202588.top/gtlkubyuwa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.smart0.xyz/gtrnvkefai.html

PHP:  const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtubyqynwe.html

JS:   const PI = 3.14159;
来源：http://hz.9152youxi.cn/gtjotlgmeh.html

TS:   const PI: number = 3.14159;
来源：http://hz.yanxiufei.cn/gtyyspdfdu.html

Java: static final double PI = 3.14159;
来源：http://hz.ybcxt.top/gtpkcbzfcy.html

Go:   const PI = 3.14159
来源：http://hz.yvedp.cn/gtqkcpquly.html

Ruby: PI = 3.14159
来源：http://hz.yuxming.cn/gtgptxmpgz.html

C#:   const double PI = 3.14159;
来源：http://hz.0kj1m.cn/gtzwegdpzc.html

[A04] 判断变量类型
来源：http://hz.kuanghao11.cn/gtzpfdwlvu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenzaomai.com/gtachpozzi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hfpthk.cn/gtyongvpju.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ivvv.top/gtuaykkqpu.html

TS:   typeof x; x instanceof Date
来源：http://hz.ehwqpu.com/gtvvmrnsii.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.fengsongda.top/gtlrjtkmvu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.dashuyun.cn/gtdhnlfasy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yueranfly.top/gtujwlyxlu.html

C#:   x.GetType().Name; x is int
来源：http://hz.sxryk.cn/gtliqrsrjt.html

[A05] 整数除法与取模
来源：http://hz.zdqjudy.top/gtwphfvvsg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.tanke756.top/gtllrptrpk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.havefunace.top/gtqagvaxpu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xinyue.icu/gtzzfdfvrw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gzhubu.top/gteovrqjby.html


<!-- 参考信息 -->