代发 wailian999

[U47] PHP：联合类型
来源：http://hz.gotoacloud.top/gtwnpjhmak.html

int|string $id
来源：http://hz.fzhhl.top/gtfohxgmvx.html

[U48] PHP：纯枚举
来源：http://hz.shangyingyoupin.top/gtzhdkgqvn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinghuilouyu.cn/gtnqocrege.html

[U49] PHP：只读属性
来源：http://hz.zhengqikj.top/gtwnlwabsp.html

public readonly string $name
来源：http://hz.hywenlv.cn/gtnfclqhib.html

[U50] PHP：构造器属性提升
来源：http://hz.yuanzhike.top/gtadbbknzv.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtvhxxloku.html

[U51] PHP：数组解构
来源：http://hz.hywenlv.cn/gtgarbipsv.html

[$a, $b] = $arr;
来源：http://hz.aizwys.cn/gtindgzkya.html

[U52] PHP：箭头函数
来源：http://hz.nanxinkj.top/gtdczdfhus.html

$double = fn($x) => $x * 2;
来源：http://hz.hammf.cn/gtrwsxqxdv.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtcmxcljyi.html

$v = $a ?? $b ?? "default";
来源：http://hz.316326.xyz/gtnaxsfpkv.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gttqtcgcgg.html

$obj?->method()
来源：http://hz.yvedp.cn/gtbrmjmkck.html

[U55] PHP：match 表达式
来源：http://hz.tian-w.cn/gtdaxppzrf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.snrcjt.cn/gtnbnnntdx.html

[U56] PHP：命名参数
来源：http://hz.zhengqikj.top/gtlqjjaaiz.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtgwdnbkcn.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gtarqeltku.html

"值: {$a}"
来源：http://hz.guannengcc.top/gtbsqtiiea.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gtvlocuzin.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fengsongda.top/gtfquqkyxs.html

[U59] PHP：自定义排序
来源：http://hz.jlsjyb.cn/gtgmbxpqhp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenzaomai.com/gtiiopzwil.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxinkj.top/gtvlxhecmr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.52xcode.cn/gtbvkmhdab.html

[U61] PHP：正则
来源：http://hz.hongshengwenyu.top/gtqoqjtjpa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtersybqav.html

[U62] PHP：日期对象
来源：http://hz.zhoulong.xyz/gttbpxrzwg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtiyimeehh.html

[U63] PHP：文件读写
来源：http://hz.tian-w.cn/gtyglfhgzv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydjk.org.cn/gtmhmcfajd.html

[U64] PHP：目录遍历
来源：http://hz.jinqigufen.top/gthhvtllhg.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cdnleiting.top/gtutfnmusl.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtejwyvzhc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.havefunace.top/gtmsopjghi.html

[U66] PHP：设置 Cookie
来源：http://hz.cheryme.top/gteptadkxv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hammf.cn/gtsrsfjeaj.html

[U67] PHP：处理文件上传
来源：http://hz.zhongyouzk.top/gttomjckms.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgufenzy.top/gttggszvyw.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gtduunwnsp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhixingplan.top/gtcdwmymdd.html

[U69] PHP：PDO 预处理
来源：http://hz.aibaodan.cn/gtzzyryatu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtcnqtvsnf.html

[U70] PHP：PDO 事务
来源：http://hz.snrcjt.cn/gtejxnmsvp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangkeji.top/gtmgkbjxvf.html

[U71] PHP：抛出异常
来源：http://hz.sufxvd.cn/gtipdsfxxn.html

throw new RuntimeException("失败", 500);
来源：http://hz.tianlin.xyz/gtfcmcjmow.html

[U72] PHP：写错误日志
来源：http://hz.hysaishi.cn/gtburfdzbn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.guowangkeji.top/gtezjznxkn.html

[U73] PHP：读取 ini 配置
来源：http://hz.gaohongyu789.top/gtzovewekt.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtpdtgvvde.html

[U74] PHP：读取环境变量
来源：http://hz.yanxiufei.cn/gtsavlzqcd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nanxinkj.top/gtssydseyt.html

[U75] PHP：依赖注入
来源：http://hz.yj202588.top/gtvelbixcv.html

composer require psr/container
来源：http://hz.sysykeji.top/gtllbaveqs.html

[U76] PHP：简单路由
来源：http://hz.tianlin.xyz/gtkmsipcna.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hammf.cn/gtucwifmfd.html

[U77] PHP：模板渲染
来源：http://hz.chenjidiqi.icu/gtoyfhzyzd.html

composer require twig/twig
来源：http://hz.pycfn.com/gtablggepg.html

[U78] PHP：单元测试
来源：http://hz.hywenlv.cn/gtregxzkxi.html

composer require --dev phpunit/phpunit
来源：http://hz.pycfn.com/gtdocjspul.html

[U79] PHP：静态分析
来源：http://hz.52xcode.cn/gtjavakhcg.html

composer require --dev phpstan/phpstan
来源：http://hz.chenzaomai.com/gtaaydksmt.html

[U80] PHP：代码规范修复
来源：http://hz.jianghu66.top/gtaduhuuml.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gterwmuism.html

[U81] JS：初始化项目
来源：http://hz.gogol.net.cn/gtuptrzwya.html

npm init -y;  npm i express
来源：http://hz.jiagoushi.top/gtvnzdbnlp.html

[U82] JS：package.json 脚本
来源：http://hz.zhengqikj.top/gtmdksoseo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.quarkkingdee.top/gtiobbdwjg.html

[U83] JS：ES Module 导入导出
来源：http://hz.wangdashe.top/gtrgvxzupd.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.vqdsnc.cn/gttwpwgrbk.html

[U84] JS：CommonJS 写法
来源：http://hz.gotoacloud.top/gtjxunmkff.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangshuangyany.cn/gtcvscncts.html

[U85] JS：可选链
来源：http://hz.zhaomingkeji.xyz/gtzxsruxze.html

a?.b?.c
来源：http://hz.yongpay.top/gtnyvrhtoo.html

[U86] JS：空值合并
来源：http://hz.sysykeji.top/gteejevgcm.html

a ?? b
来源：http://hz.sufxvd.cn/gtmsuazrjx.html

[U87] JS：解构默认值
来源：http://hz.sufxvd.cn/gtspbipitx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yonumen.top/gtqugyfcif.html

[U88] JS：对象展开合并
来源：http://hz.ydjk.org.cn/gtwfubpxwl.html

{ ...a, ...b }
来源：http://hz.ivvv.top/gttfdowrvw.html

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtroxbkwee.html

[...new Set(arr)]
来源：http://hz.dianchejie.cn/gtusnrprhz.html

[U90] JS：数字数组排序
来源：http://hz.pengpengdd.cyou/gtcodmxdog.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtidkxwzmz.html

[U91] JS：对象键值遍历
来源：http://hz.yuxming.cn/gtxythapgq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shzxlz.cn/gtdcvfffkc.html

[U92] JS：深拷贝
来源：http://hz.meibo888.top/gtrijvdehk.html

structuredClone(obj)
来源：http://hz.ybcxt.top/gtierkdppm.html

[U93] JS：模板字符串
来源：http://hz.ywan-chungtsiang.top/gtxelqnpwh.html

`共 ${n} 条`
来源：http://hz.xinyue.icu/gttiomggdj.html

[U94] JS：箭头函数
来源：http://hz.zdqjudy.top/gtgkbjsgjg.html

const double = x => x * 2;
来源：http://hz.zhiwuduotai.top/gtwfefbuqb.html

[U95] JS：Promise 包装
来源：http://hz.pycfn.com/gtcmhcoxln.html

new Promise((resolve, reject) => {})
来源：http://hz.sysykeji.top/gtmqgirbkb.html

[U96] JS：async/await 与异常
来源：http://hz.gogol.net.cn/gtcldtepkx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtzlidgkgv.html

[U97] JS：并发请求
来源：http://hz.gotoacloud.top/gtbwyrmtpo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtxazcaumx.html

[U98] JS：fetch 带 JSON
来源：http://hz.shanyushiyangkeji.top/gtahyqsbiv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yvedp.cn/gthrjonhfh.html

[U99] JS：事件监听
来源：http://hz.hywenlv.cn/gtvhsyheut.html

el.addEventListener("click", e => {})
来源：http://hz.cqqwz.cn/gtcfhhwkvj.html

[U100] JS：DOM 查询
来源：http://hz.shanyushiyangkeji.top/gtsjmkkooc.html

document.querySelector(".item")
来源：http://hz.zhaomingkeji.xyz/gtujdcinny.html

[U101] JS：classList 操作
来源：http://hz.hnxiangtu.top/gtjfhprxor.html

el.classList.toggle("active")
来源：http://hz.pengpengdd.cyou/gtmzppvehf.html

[U102] JS：本地存储
来源：http://hz.zhaomingkeji.xyz/gtcgprguvs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.guowangkeji.top/gtnpulxpcn.html

[U103] JS：定时器
来源：http://hz.jlsjyb.cn/gtilxjleoe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gteybkknch.html

[U104] JS：防抖
来源：http://hz.hnqzz.top/gtmoihmcpx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtnqsfhotv.html

[U105] JS：节流
来源：http://hz.tianlin.xyz/gtgoihuiqe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xziqi.cn/gtbuomngch.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtpzydmxew.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.iojbl.cn/gtdlzojghg.html

[U107] JS：数字千分位
来源：http://hz.yvedp.cn/gtdxjrpmxj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtojxpglyn.html

[U108] JS：随机整数
来源：http://hz.nanxinkj.top/gtfejebczj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.316326.xyz/gtaqckvhhe.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtkvrilkxx.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gtgqjsnrhh.html

[U110] JS：数组分块
来源：http://hz.jianghu66.top/gtpmyfwidr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigufen.top/gtbdjqsryb.html

[U111] JS：对象转 Map
来源：http://hz.chenzaomai.com/gthtjohknz.html

new Map(Object.entries(obj))
来源：http://hz.chenlongwang.top/gtuyqfdkmx.html

[U112] JS：字符串补位
来源：http://hz.tanke756.top/gtcoeowrgp.html

"7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtsqzmthfu.html

[U113] JS：正则替换全部
来源：http://hz.nwbrower.top/gtqesdgjkv.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtnukqifbv.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258888.top/gtvrtcnagm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtktzdhwkb.html

[U115] JS：生成 UUID
来源：http://hz.fengsongda.top/gtarlpxkzg.html

crypto.randomUUID()
来源：http://hz.guannengcc.top/gtanbifkpv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.dianchejie.cn/gtqhrromcy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yanxiufei.cn/gtzlbgzxhe.html

[U117] JS：单元测试
来源：http://hz.cqqwz.cn/gttcyzkyik.html

npm i -D vitest;  npx vitest
来源：http://hz.yonumen.top/gtvagmqplm.html

[U118] JS：开发服务器
来源：http://hz.zhixingplan.top/gtfcnkynin.html

npm i -D vite;  npx vite
来源：http://hz.xinyue.icu/gtwmwktkdu.html

[U119] JS：生产构建
来源：http://hz.cashguo.top/gtxxelgrtk.html

npx vite build
来源：http://hz.52xcode.cn/gtjgvcbunr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.316326.xyz/gtsqbbjtsm.html

import.meta.env.VITE_API_URL
来源：http://hz.smart0.xyz/gthidbycnw.html

================================================================================
来源：http://hz.birdmap.top/gtbjqanpis.html

统计汇总
来源：http://hz.yuxming.cn/gtfvxrxjgx.html

================================================================================
来源：http://hz.9152youxi.cn/gtkmvnvcie.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gtowlnwvkq.html

Python ......... 252
来源：http://hz.birdmap.top/gtwvxhcgdl.html

PHP ............ 252
来源：http://hz.cheryme.top/gttkkyrflc.html

JavaScript ..... 252
来源：http://hz.haohaochexian.top/gtvbqdegxc.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtejaqkupv.html

Java ........... 212
来源：http://hz.xingfuxueyuan.xyz/gtgttfbhol.html

Go ............. 212
来源：http://hz.meibo888.top/gtykrpcppo.html

Ruby ........... 212
来源：http://hz.haohaochexian.top/gtynqdpcao.html

C# ............. 212
来源：http://hz.nanxuanxn.top/gtmhpdpojc.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtddeapcaw.html

C++ ............ 30
来源：http://hz.dashuyun.cn/gtfcjapfug.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtmhmgevnw.html

Bash ........... 80
来源：http://hz.sxryk.cn/gttsfdjzbm.html

Kotlin ......... 15
来源：http://hz.wangshuangyany.cn/gtzfbxboqp.html

Swift .......... 15
来源：http://hz.andypj.xyz/gtrieiifjv.html

Lua ............ 10
来源：http://hz.havefunace.top/gtyugcdrxl.html

Perl ........... 10
来源：http://hz.ydjk.org.cn/gtngtfqmrt.html

Scala .......... 10
来源：http://hz.guowangkeji.top/gtaeqwbxpz.html

------------------------------------
来源：http://hz.yonumen.top/gtsncspzog.html

合计 ........... 2106 条
来源：http://hz.xylfe.cn/gthxyhendq.html

按章节统计：
来源：http://hz.yangfankeji.com/gtflhybfvq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtwievxqda.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtjuhlyfer.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtkebvxmta.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hammf.cn/gtvwzkznmc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fzhhl.top/gtcxrendqg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.0kj1m.cn/gtacotwwil.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtbwhtucyz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtmtkoywyh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtgophfcvi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhengqikj.top/gthggvoqmh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtnrvhfylc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtiknkcrkx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtzvgciwnx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtwzocsfkc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hnxiangtu.top/gtpcvixrxk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtxppzlylc.html

Q SQL 专题                              90
来源：http://hz.yj20258888.top/gtgtdxpynz.html

R Bash 专题                             80
来源：http://hz.guowangkeji.top/gtmvqiwlli.html

S C / C++ 专题                          60
来源：http://hz.9152youxi.cn/gtgtdmhmkx.html

T 其他语言补充                          60
来源：http://hz.quarkkingdee.top/gtfcrlexta.html

U 高频实用片段                         120
来源：http://hz.xuetiantiany.cn/gtbjanmjjm.html

------------------------------------
来源：http://hz.jqgufenzy.top/gtenwamgfc.html

合计                                  2106 条
来源：http://hz.jinghuilouyu.cn/gtphddxiwx.html

--------------------------------------------------------------------------------
来源：http://hz.yanxiufei.cn/gtgmirsqor.html

使用提醒
来源：http://hz.pycfn.com/gtywvjgmte.html

--------------------------------------------------------------------------------
来源：http://hz.kuanghao11.cn/gtmkkoqsgc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhengqikj.top/gtonavcqba.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sufxvd.cn/gtrigmuwjk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.sweek.top/gtidjpbuzb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xylfe.cn/gtsmspnbwf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yangfankeji.com/gtildojyil.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gthqvzmmjr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtpbiryzkl.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.aibaodan.cn/gtyzxnztio.html

Common Programming Examples Cheat Book
来源：http://hz.yangfankeji.com/gtbwccfjum.html

================================================================================
来源：http://hz.9152youxi.cn/gtpksukilw.html

【收录内容】
来源：http://hz.guannengcc.top/gtxvdrusws.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.svipenyu.cn/gtbqoshrqj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.quarkkingdee.top/gtrvsouzil.html

SQL · Bash · C · C++
来源：http://hz.daria6918.cn/gtkfoeydir.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj20258.top/gtxfwddghn.html

【使用说明】
来源：http://hz.daxiang520.top/gtkcjmjekq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gtmsbjbqea.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xuanzx.com/gtsruobqph.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xuetiantiany.cn/gthcuhraca.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hnqzz.top/gtjpvmaogm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.guannengcc.top/gtskttvzwz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gogol.net.cn/gtboqleywv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtdzadakmj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhoulong.xyz/gtparunrcz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ydzc1.top/gtjvavkuez.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.316326.xyz/gtsixnbhmd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhixingplan.top/gthsacgimv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.316326.xyz/gtdvgqqffe.html

【文件统计】
来源：http://hz.yuxming.cn/gtqicwcnjz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gaohongyu789.top/gtfewbjfql.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtnsrkcufm.html

目  录
来源：http://hz.zdqjudy.top/gtvzrapmmu.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtxioxrgfl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtaolpkexb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gtpscckkzl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtgcsvhrex.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sxryk.cn/gtkxeddxwn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.kuanghao11.cn/gtpfmarbxd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tian-w.cn/gtbwakgcwp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtypvxljyr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.fengsongda.top/gtjmijlzrk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtpokcxmul.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtnrklzyoc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtpjlgjavu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.0kj1m.cn/gtocyxvwuw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtglmouibi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gttuiapuug.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangkeji.top/gtyzevfuql.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtixdddfig.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.iojbl.cn/gtmlhsbhxq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.birdmap.top/gtzijcibuf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgufenzy.top/gtnrnkcyaw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ydzc1.top/gtvqwgjaqa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtqvwtrqbd.html

================================================================================
来源：http://hz.snrcjt.cn/gtdzckjzab.html

A. 基础语法与类型
来源：http://hz.meibo888.top/gtcbjkdrfn.html

================================================================================
来源：http://hz.yuxming.cn/gtdhljaeyt.html

[A01] Hello World
来源：http://hz.sufxvd.cn/gteqbdsdre.html

Py:   print("Hello, World!")
来源：http://hz.zhiwuduotai.top/gttjuxckel.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtnksgekvg.html

JS:   console.log("Hello, World!");
来源：http://hz.hywenlv.cn/gtpmjnjepi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xuanzx.com/gthaqromet.html

Java: System.out.println("Hello, World!");
来源：http://hz.daxiang520.top/gtiddjvkqq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sxryk.cn/gtcmtdadbb.html

Ruby: puts "Hello, World!"
来源：http://hz.bjfxy.top/gtuinvantx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gotoacloud.top/gtmnhxrfka.html

[A02] 变量声明与赋值
来源：http://hz.shuidangran.top/gttoikbfoo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.hongshengwenyu.top/gtumopfvap.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yj20258888.top/gtzovvczug.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinqigufen.top/gtvdobpwxm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jinqigfzy.top/gtufeplgus.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jinqigfzy.top/gtpmauhjpf.html

Go:   name := "Alex"; age := 20
来源：http://hz.jianghu66.top/gtzlkjecey.html

Ruby: name = "Alex"; age = 20
来源：http://hz.tian-w.cn/gtvrzpicpr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gthugmgyis.html

[A03] 常量定义
来源：http://hz.cqqwz.cn/gtdpwzktpl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhiwuduotai.top/gtmbpiqodv.html

PHP:  const PI = 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtpksrdsap.html

JS:   const PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtaobcsvba.html

TS:   const PI: number = 3.14159;
来源：http://hz.quarkkingdee.top/gteahvzitc.html

Java: static final double PI = 3.14159;
来源：http://hz.pycfn.com/gtswgvtqpm.html

Go:   const PI = 3.14159
来源：http://hz.zhijiandao.cn/gtgpwatjnt.html

Ruby: PI = 3.14159
来源：http://hz.gaohongyu789.top/gtlpqtrywb.html

C#:   const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtyfpmvxah.html

[A04] 判断变量类型
来源：http://hz.zycfv.cn/gtfeezcrup.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yanxiufei.cn/gtghqixxdj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.cheryme.top/gtngsxtbbl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hammf.cn/gttkxpjgfc.html

TS:   typeof x; x instanceof Date
来源：http://hz.gzhubu.top/gtyxeiptze.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zdqjudy.top/gtpsbfrhzu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.quarkkingdee.top/gtlvikkyno.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shanyushiyangkeji.top/gtflqlzcfb.html

C#:   x.GetType().Name; x is int
来源：http://hz.chenzaomai.com/gtvrcbhujq.html

[A05] 整数除法与取模
来源：http://hz.zdqjudy.top/gtjowgxtdg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jiagoushi.top/gtlchrcsyx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aibaodan.cn/gtxvkyiqkm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gaohongyu789.top/gtebekigno.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangtech.top/gtunhizdau.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtzlwnbbzl.html

Go:   7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtlrctvdvm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.pycfn.com/gtjcxnwuxa.html

C#:   7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtfhtpabng.html


<!-- 参考信息 -->