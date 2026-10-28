代发 wailian999

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gtbmyuyrdp.html

int|string $id
来源：http://hz.daria6918.cn/gtombnrtrr.html

[U48] PHP：纯枚举
来源：http://hz.svipenyu.cn/gtpnxxlqxe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258.top/gtodrtlmkv.html

[U49] PHP：只读属性
来源：http://hz.hfpthk.cn/gteqnagpkl.html

public readonly string $name
来源：http://hz.nwbrower.top/gtcawlzvxs.html

[U50] PHP：构造器属性提升
来源：http://hz.gogol.net.cn/gtpusjrfll.html

public function __construct(private int $id) {}
来源：http://hz.wangshuangyany.cn/gttrtyalfw.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtpjtoizwb.html

[$a, $b] = $arr;
来源：http://hz.yvedp.cn/gtqbmvtpsb.html

[U52] PHP：箭头函数
来源：http://hz.zhongyouzk.top/gtdotzvojm.html

$double = fn($x) => $x * 2;
来源：http://hz.yangfankeji.com/gtjsmsqpdn.html

[U53] PHP：空合并运算符
来源：http://hz.jinghuilouyu.cn/gtpbpvewbe.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuanzx.com/gtfbennzvl.html

[U54] PHP：空安全调用
来源：http://hz.ppjwa.cn/gtphhnftxy.html

$obj?->method()
来源：http://hz.meibo888.top/gtkaakehqg.html

[U55] PHP：match 表达式
来源：http://hz.xingfuxueyuan.xyz/gtjozdfuzq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.birdmap.top/gtyowhgoij.html

[U56] PHP：命名参数
来源：http://hz.0kj1m.cn/gtwylsecmp.html

f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtiwamewns.html

[U57] PHP：字符串插值
来源：http://hz.xziqi.cn/gtdqbumkev.html

"值: {$a}"
来源：http://hz.shzxlz.cn/gtcwzddszh.html

[U58] PHP：数组三件套
来源：http://hz.bjfxy.top/gtasmndmcr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhaomingkeji.xyz/gtvsqbyjwh.html

[U59] PHP：自定义排序
来源：http://hz.yangfankeji.com/gtpheonbxf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtlkifebno.html

[U60] PHP：JSON 编解码
来源：http://hz.birdmap.top/gtmcfhvagv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ybcxt.top/gtzgavlwuq.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtvwopovfh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtazawgrrs.html

[U62] PHP：日期对象
来源：http://hz.jlsjyb.cn/gtkjdmpaur.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gotoacloud.top/gteggzrdck.html

[U63] PHP：文件读写
来源：http://hz.jyoumei.cn/gtckcsvdxh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tianlin.xyz/gtdxbadbgg.html

[U64] PHP：目录遍历
来源：http://hz.sxryk.cn/gtcdjdwzfq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtizgayenk.html

[U65] PHP：会话
来源：http://hz.guowangkeji.top/gtzckqdaoa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.9152youxi.cn/gtxnfzyxzr.html

[U66] PHP：设置 Cookie
来源：http://hz.gaohongyu789.top/gtpjdlmoua.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtpesojldi.html

[U67] PHP：处理文件上传
来源：http://hz.yangfankeji.com/gtwravkmfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangshuangyany.cn/gthydxbpzg.html

[U68] PHP：PDO 连接
来源：http://hz.xingfuxueyuan.xyz/gtvsvkjcsz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aibaodan.cn/gtjhmdrouv.html

[U69] PHP：PDO 预处理
来源：http://hz.hnqzz.top/gtmdoabeip.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.smart0.xyz/gtekwbobtv.html

[U70] PHP：PDO 事务
来源：http://hz.zhengqikj.top/gtcduikpxz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.redwolf501.top/gtuwskdchx.html

[U71] PHP：抛出异常
来源：http://hz.yonumen.top/gtoaumxuvk.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinqigufen.top/gtqjydrsbr.html

[U72] PHP：写错误日志
来源：http://hz.fengsongda.top/gtmokdkigc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhoulong.xyz/gtexqykdvk.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydzc1.top/gtqusbfwmb.html

parse_ini_file("config.ini", true)
来源：http://hz.zdqjudy.top/gtbynfdrvz.html

[U74] PHP：读取环境变量
来源：http://hz.c1oappe.top/gtgtxfyrqi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.wangdashe.top/gtjgtsbtcs.html

[U75] PHP：依赖注入
来源：http://hz.fzhhl.top/gtwhorviet.html

composer require psr/container
来源：http://hz.chenjidiqi.icu/gtnoluwwrt.html

[U76] PHP：简单路由
来源：http://hz.yuanzhike.top/gtpjjtsjxi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.fengsongda.top/gtkjmcjpdu.html

[U77] PHP：模板渲染
来源：http://hz.hongshengwenyu.top/gtmwcggchz.html

composer require twig/twig
来源：http://hz.hnxiangtu.top/gtkhukcelp.html

[U78] PHP：单元测试
来源：http://hz.yj202588.top/gtewnotcnw.html

composer require --dev phpunit/phpunit
来源：http://hz.gogol.net.cn/gtteezngol.html

[U79] PHP：静态分析
来源：http://hz.yueranfly.top/gtrhvlgudz.html

composer require --dev phpstan/phpstan
来源：http://hz.shanyushiyangtech.top/gtaxkfvhey.html

[U80] PHP：代码规范修复
来源：http://hz.zdqjudy.top/gtbegdwtts.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yj20258.top/gtlpxczxxu.html

[U81] JS：初始化项目
来源：http://hz.xziqi.cn/gtnhckwnnq.html

npm init -y;  npm i express
来源：http://hz.ehwqpu.com/gtuzbalxyv.html

[U82] JS：package.json 脚本
来源：http://hz.sxryk.cn/gtntvfxxdg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yj20258888.top/gtrvkobtgs.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtvxbqvlai.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhixingplan.top/gtiunfphch.html

[U84] JS：CommonJS 写法
来源：http://hz.xylfe.cn/gtbtybsoek.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.pengpengdd.cyou/gtfcmjytzg.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtmotlkexz.html

a?.b?.c
来源：http://hz.andypj.xyz/gtcksjblxt.html

[U86] JS：空值合并
来源：http://hz.meibo888.top/gtdpfoidte.html

a ?? b
来源：http://hz.jyoumei.cn/gthqwxrquf.html

[U87] JS：解构默认值
来源：http://hz.52xcode.cn/gtjznftgqk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.52xcode.cn/gtnzljbgkz.html

[U88] JS：对象展开合并
来源：http://hz.aizwys.cn/gtmxgyjmup.html

{ ...a, ...b }
来源：http://hz.hnqzz.top/gtzpxnxwrk.html

[U89] JS：数组去重
来源：http://hz.jqgfzy.top/gtgvovnpui.html

[...new Set(arr)]
来源：http://hz.iojbl.cn/gtwxqcdjaf.html

[U90] JS：数字数组排序
来源：http://hz.xziqi.cn/gtxkqersdi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtzoyghqpu.html

[U91] JS：对象键值遍历
来源：http://hz.bjfxy.top/gthojuwbig.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenjidiqi.icu/gtvqblphkl.html

[U92] JS：深拷贝
来源：http://hz.daria6918.cn/gtjixehonr.html

structuredClone(obj)
来源：http://hz.yangfankeji.com/gtubkxncdw.html

[U93] JS：模板字符串
来源：http://hz.zhiwuduotai.top/gtaqomnfgh.html

`共 ${n} 条`
来源：http://hz.ydzc1.top/gttsxrrope.html

[U94] JS：箭头函数
来源：http://hz.shangyingyoupin.top/gtrnzzqymv.html

const double = x => x * 2;
来源：http://hz.zycfv.cn/gthrccxnyx.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangkeji.top/gtmynqtges.html

new Promise((resolve, reject) => {})
来源：http://hz.gzhubu.top/gtlomxwvri.html

[U96] JS：async/await 与异常
来源：http://hz.xuetiantiany.cn/gtxjvwvjhs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtgtkowfvd.html

[U97] JS：并发请求
来源：http://hz.jianghu66.top/gtaipycyva.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtsklnjdlr.html

[U98] JS：fetch 带 JSON
来源：http://hz.zycfv.cn/gtksiyqyxx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.pengpengdd.cyou/gtqjobdsuh.html

[U99] JS：事件监听
来源：http://hz.yvedp.cn/gtfegddcjp.html

el.addEventListener("click", e => {})
来源：http://hz.nwbrower.top/gtakyjbkfy.html

[U100] JS：DOM 查询
来源：http://hz.xuanzx.com/gtiqvhpjrp.html

document.querySelector(".item")
来源：http://hz.mhx1999.top/gtboqjjehg.html

[U101] JS：classList 操作
来源：http://hz.fengsongda.top/gtqxvsbebf.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtosrvmuli.html

[U102] JS：本地存储
来源：http://hz.yj20258888.top/gtzgfjzbnw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.sysykeji.top/gtbndohtjv.html

[U103] JS：定时器
来源：http://hz.dianchejie.cn/gtblqxnpie.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yuxming.cn/gtdlrnrqhn.html

[U104] JS：防抖
来源：http://hz.jyoumei.cn/gtpkxpuwlq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ywan-chungtsiang.top/gtdbtpwhvg.html

[U105] JS：节流
来源：http://hz.dianchejie.cn/gtfzetlslk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydjk.org.cn/gtazblpcgk.html

[U106] JS：日期格式化
来源：http://hz.dianchejie.cn/gtaitkztcy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shuidangran.top/gttugjjpod.html

[U107] JS：数字千分位
来源：http://hz.yvedp.cn/gtrwxsouct.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuanzhike.top/gtpcbhhivr.html

[U108] JS：随机整数
来源：http://hz.feifeiyinyue.top/gtkhglxipo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gotoacloud.top/gtxpzahwyd.html

[U109] JS：数组分组
来源：http://hz.guowangkeji.top/gtsribecsg.html

Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gtqolnnmsm.html

[U110] JS：数组分块
来源：http://hz.shangyingyoupin.top/gtrggdggro.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ivvv.top/gthubhqlys.html

[U111] JS：对象转 Map
来源：http://hz.shuidangran.top/gtovqvjahv.html

new Map(Object.entries(obj))
来源：http://hz.cdnleiting.top/gtdtjvkfuf.html

[U112] JS：字符串补位
来源：http://hz.havefunace.top/gtrrtafafd.html

"7".padStart(3, "0")
来源：http://hz.316326.xyz/gtkmdtuyud.html

[U113] JS：正则替换全部
来源：http://hz.yuanzhike.top/gtotoeyaod.html

s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtyedfjoaw.html

[U114] JS：JSON 深比较
来源：http://hz.jianghu66.top/gtkxstjzff.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenjidiqi.icu/gtbugtbxmw.html

[U115] JS：生成 UUID
来源：http://hz.yangfankeji.com/gtvdnrdlag.html

crypto.randomUUID()
来源：http://hz.fzhhl.top/gtiskbameh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.316326.xyz/gtxkxsbegi.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cqqwz.cn/gtswxcdzyz.html

[U117] JS：单元测试
来源：http://hz.chenjidiqi.icu/gtybfgzjuw.html

npm i -D vitest;  npx vitest
来源：http://hz.yongpay.top/gtvbkeblbj.html

[U118] JS：开发服务器
来源：http://hz.chenjidiqi.icu/gtakuhtbro.html

npm i -D vite;  npx vite
来源：http://hz.xinyue.icu/gtpajdtmlx.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtkusbhcid.html

npx vite build
来源：http://hz.ivvv.top/gtezuaqphz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.cqqwz.cn/gtrosohtke.html

import.meta.env.VITE_API_URL
来源：http://hz.sufxvd.cn/gtufcuxwje.html

================================================================================
来源：http://hz.guowangkeji.top/gtetslkmow.html

统计汇总
来源：http://hz.tanke756.top/gtjymedqed.html

================================================================================
来源：http://hz.zdqjudy.top/gtvdzdffpz.html

按语言统计（条）：
来源：http://hz.dianchejie.cn/gtjnbjyqse.html

Python ......... 252
来源：http://hz.shuidangran.top/gtvwdzusdk.html

PHP ............ 252
来源：http://hz.yanxiufei.cn/gtetbelbxe.html

JavaScript ..... 252
来源：http://hz.guowangkeji.top/gtdahivfbe.html

TypeScript ..... 212
来源：http://hz.jianghu66.top/gtgfrqarmz.html

Java ........... 212
来源：http://hz.jiagoushi.top/gtzlqxzhgs.html

Go ............. 212
来源：http://hz.meibo888.top/gtlryyemkb.html

Ruby ........... 212
来源：http://hz.fzhhl.top/gtcwmtjvuc.html

C# ............. 212
来源：http://hz.xylfe.cn/gttecsfqrt.html

C .............. 30
来源：http://hz.yonumen.top/gttobkqdzc.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gthmnbaojc.html

SQL ............ 90
来源：http://hz.iojbl.cn/gtrsxjakhw.html

Bash ........... 80
来源：http://hz.sxryk.cn/gtwlwsimoq.html

Kotlin ......... 15
来源：http://hz.guowangkeji.top/gtnerwskpd.html

Swift .......... 15
来源：http://hz.meibo888.top/gtmagfxxqi.html

Lua ............ 10
来源：http://hz.shuidangran.top/gtoelctulg.html

Perl ........... 10
来源：http://hz.yangfankeji.com/gteakwqodi.html

Scala .......... 10
来源：http://hz.xziqi.cn/gtqpqbnqud.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtxvrkxwxj.html

合计 ........... 2106 条
来源：http://hz.xuetiantiany.cn/gtrdqxhepq.html

按章节统计：
来源：http://hz.vqdsnc.cn/gtyokecmsw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtqxuinfzp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tianlin.xyz/gtwfhmaclp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gthavkqdxd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtuabcghif.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cheryme.top/gtssytyyqv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zycfv.cn/gtgouyxojs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yanxiufei.cn/gtpqnzroof.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.fengsongda.top/gterwxafmt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtkcxcoqos.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhongyouzk.top/gtdwehlftm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtpnuejhnk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtyhjvlhpa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtopanmtbd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj20258.top/gtvhefjagf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.gogol.net.cn/gtelmvykcl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtnypfnahm.html

Q SQL 专题                              90
来源：http://hz.bjfxy.top/gtaogkhcjp.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gtwjssglff.html

S C / C++ 专题                          60
来源：http://hz.birdmap.top/gthvysaovq.html

T 其他语言补充                          60
来源：http://hz.nanxinkj.top/gtmrjiundm.html

U 高频实用片段                         120
来源：http://hz.sxryk.cn/gtfsuykvva.html

------------------------------------
来源：http://hz.hnqzz.top/gteupvugyo.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtubjittbe.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtjywghzaz.html

使用提醒
来源：http://hz.kuanghao11.cn/gtyttwqjfy.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtktrynapr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.9152youxi.cn/gttlcagfgz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuxming.cn/gtfgvbcyva.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gogol.net.cn/gtaghinwjb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.mhx1999.top/gtsaxtdknx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zdqjudy.top/gtdznpdelj.html

—— 文件结束 ——
来源：http://hz.yvedp.cn/gtbmjimnsg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjsxbvgfj.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jiagoushi.top/gthetmxvwh.html

Common Programming Examples Cheat Book
来源：http://hz.pengpengdd.cyou/gtsvgasfqu.html

================================================================================
来源：http://hz.yj20258.top/gtnftdtqwg.html

【收录内容】
来源：http://hz.hywenlv.cn/gtzvjpucch.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.wangdashe.top/gtcnjtuqdx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fzhhl.top/gttjxwmsht.html

SQL · Bash · C · C++
来源：http://hz.yongpay.top/gtrggvzmmp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xylfe.cn/gttyfqaukq.html

【使用说明】
来源：http://hz.hnxiangtu.top/gtkbzcdtqb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.cucudq.cn/gtpsqowupm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hnxiangtu.top/gtlfihqvde.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhiwuduotai.top/gtdplkkzwt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhiwuduotai.top/gtrpxgufxj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtdgklpcmb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.c1oappe.top/gtsboxrfou.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangdashe.top/gtcoiwhsjk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xziqi.cn/gtequkolok.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.aizwys.cn/gtluyutvwi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.andypj.xyz/gtqaesptbq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hammf.cn/gtcliikdod.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xziqi.cn/gtajdukhif.html

【文件统计】
来源：http://hz.shanyushiyangkeji.top/gtwftlwhnb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gzhubu.top/gttfybrafy.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtmvqjuwxh.html

目  录
来源：http://hz.ppjwa.cn/gtinspxoyc.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtrjlvumbr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtooizabdz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtgkiyguth.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sweek.top/gtqsxgitsc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cheryme.top/gtqonuzynv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.chenlongwang.top/gttemsdbql.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtxuvyqnna.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.quarkkingdee.top/gtomzpnhdi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtssxpncjj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtljomkont.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtyxogmzte.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jiagoushi.top/gtcahwunfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtmogxaxia.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtajamtvzy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gtnbbtfoff.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.cheryme.top/gtuvevwcpa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtceecxtco.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangdashe.top/gtctabwyai.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.meibo888.top/gtcjjqywhz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.birdmap.top/gtxhfbquuc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangdashe.top/gtedcjsnrw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtrukadyfw.html

================================================================================
来源：http://hz.svipenyu.cn/gtbcachwhc.html

A. 基础语法与类型
来源：http://hz.pycfn.com/gtblynomdo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlukhzpcz.html

[A01] Hello World
来源：http://hz.yueranfly.top/gtmdymbneh.html

Py:   print("Hello, World!")
来源：http://hz.feifeiyinyue.top/gthnuadezo.html

PHP:  echo "Hello, World!";
来源：http://hz.hammf.cn/gtfxkafmud.html

JS:   console.log("Hello, World!");
来源：http://hz.xuetiantiany.cn/gtggcmdblg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wangdashe.top/gtiiksjfiu.html

Java: System.out.println("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtihzqzkhb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtdypirkvu.html

Ruby: puts "Hello, World!"
来源：http://hz.kuanghao11.cn/gtblbcqcau.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gtzsarnufu.html

[A02] 变量声明与赋值
来源：http://hz.cashguo.top/gtzkzhxdjq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuanzx.com/gthpqhqpaf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gtmpgzqvyb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.tian-w.cn/gtifdvyzhd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.c1oappe.top/gtsqtkrkgo.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.tian-w.cn/gtwezsvjqj.html

Go:   name := "Alex"; age := 20
来源：http://hz.shzxlz.cn/gtvpafuavl.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zycfv.cn/gtcrkwrjmy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtaolddwoj.html

[A03] 常量定义
来源：http://hz.ivvv.top/gtgbrcphmw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinghuilouyu.cn/gtxvleffqa.html

PHP:  const PI = 3.14159;
来源：http://hz.yueranfly.top/gtjpbyvhjw.html

JS:   const PI = 3.14159;
来源：http://hz.yueranfly.top/gtbvktuvxg.html

TS:   const PI: number = 3.14159;
来源：http://hz.birdmap.top/gtojgrubfv.html

Java: static final double PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtggsstlce.html

Go:   const PI = 3.14159
来源：http://hz.sweek.top/gtjzqhzmmb.html

Ruby: PI = 3.14159
来源：http://hz.chenzaomai.com/gtjmxnctns.html

C#:   const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtljgagqfx.html

[A04] 判断变量类型
来源：http://hz.yj202588.top/gtqncvxcqk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zycfv.cn/gtocetipad.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.9152youxi.cn/gttxydklzs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yuanzhike.top/gttbtqhwnz.html

TS:   typeof x; x instanceof Date
来源：http://hz.yj20258888.top/gtgfnmracm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gtefhlldkf.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hysaishi.cn/gtuopxrkmq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.fzhhl.top/gtirldttwd.html

C#:   x.GetType().Name; x is int
来源：http://hz.nwbrower.top/gtzvkpewkl.html

[A05] 整数除法与取模
来源：http://hz.yongpay.top/gtlfcczvxn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hnxiangtu.top/gtcraapjcf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yvedp.cn/gtqarzztzp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cashguo.top/gtcbyymtyi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zycfv.cn/gtkblcextp.html

Java: 7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtfyiohdjv.html

Go:   7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtpmylnmec.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtmaftdnfm.html

C#:   7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gtctlvzpmm.html


<!-- 参考信息 -->