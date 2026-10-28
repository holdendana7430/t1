代发 wailian999

[U53] PHP：空合并运算符
来源：http://hz.havefunace.top/gtmkplzzbw.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gtbklxvfzm.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtcpnzhrni.html

$obj?->method()
来源：http://hz.52xcode.cn/gtcryrtmul.html

[U55] PHP：match 表达式
来源：http://hz.birdmap.top/gtedlmfund.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gogol.net.cn/gtromysoqb.html

[U56] PHP：命名参数
来源：http://hz.ehwqpu.com/gtoyabrlyc.html

f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtgvgkxndb.html

[U57] PHP：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtrskvakgm.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtjgxzjpex.html

[U58] PHP：数组三件套
来源：http://hz.yueranfly.top/gtfrlvqmio.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj202588.top/gtxatkxast.html

[U59] PHP：自定义排序
来源：http://hz.jinghuilouyu.cn/gtladewzvo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtysfaghwt.html

[U60] PHP：JSON 编解码
来源：http://hz.hongshengwenyu.top/gtzhvuadpo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yanxiufei.cn/gtybdxgfmc.html

[U61] PHP：正则
来源：http://hz.hfpthk.cn/gtsdlklscv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtgmbbruej.html

[U62] PHP：日期对象
来源：http://hz.guowangkeji.top/gtudmmefmo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jqgufenzy.top/gtbdxjsnik.html

[U63] PHP：文件读写
来源：http://hz.redwolf501.top/gtbovxqsaw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.quarkkingdee.top/gtdaieetir.html

[U64] PHP：目录遍历
来源：http://hz.cheryme.top/gtfegmcquo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gthbfzrjem.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gtumtcoqit.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ppjwa.cn/gteqlkogxr.html

[U66] PHP：设置 Cookie
来源：http://hz.sweek.top/gtyqwubnun.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.pengpengdd.cyou/gtygolguot.html

[U67] PHP：处理文件上传
来源：http://hz.xingfuxueyuan.xyz/gtxvtbvosx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shanyushiyangkeji.top/gtinqeimcy.html

[U68] PHP：PDO 连接
来源：http://hz.sweek.top/gtmymhbeix.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jqgfzy.top/gtuxwrmpzo.html

[U69] PHP：PDO 预处理
来源：http://hz.hnxiangtu.top/gtmsqokiuj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinqigfzy.top/gtembojxxf.html

[U70] PHP：PDO 事务
来源：http://hz.cucudq.cn/gtmsbnorpk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yanxiufei.cn/gtgahzvgeg.html

[U71] PHP：抛出异常
来源：http://hz.xinyue.icu/gtkdlmtftm.html

throw new RuntimeException("失败", 500);
来源：http://hz.cdnleiting.top/gtdiwsieid.html

[U72] PHP：写错误日志
来源：http://hz.bjfxy.top/gthhlvftlp.html

error_log("失败: " . $e->getMessage());
来源：http://hz.snrcjt.cn/gtcnlijkir.html

[U73] PHP：读取 ini 配置
来源：http://hz.dashuyun.cn/gtbnjkputu.html

parse_ini_file("config.ini", true)
来源：http://hz.ydzc1.top/gtmjmgvrza.html

[U74] PHP：读取环境变量
来源：http://hz.jianghu66.top/gtgcnrhovl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jlsjyb.cn/gtwipvrtwf.html

[U75] PHP：依赖注入
来源：http://hz.xinyue.icu/gtiktrfcpu.html

composer require psr/container
来源：http://hz.fzhhl.top/gtgbjfruqt.html

[U76] PHP：简单路由
来源：http://hz.zhoulong.xyz/gtcgxipyql.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cdnleiting.top/gtrabskcub.html

[U77] PHP：模板渲染
来源：http://hz.ppjwa.cn/gtfsqntile.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtuuaiwcev.html

[U78] PHP：单元测试
来源：http://hz.nwbrower.top/gtphjkvvts.html

composer require --dev phpunit/phpunit
来源：http://hz.0kj1m.cn/gtwytoqzdo.html

[U79] PHP：静态分析
来源：http://hz.meibo888.top/gtdttetoeg.html

composer require --dev phpstan/phpstan
来源：http://hz.sysykeji.top/gtlerurffi.html

[U80] PHP：代码规范修复
来源：http://hz.havefunace.top/gtitoalbvk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.daria6918.cn/gtykaxxjfr.html

[U81] JS：初始化项目
来源：http://hz.nanxinkj.top/gtwznchxkx.html

npm init -y;  npm i express
来源：http://hz.sufxvd.cn/gtdpwfooaz.html

[U82] JS：package.json 脚本
来源：http://hz.vqdsnc.cn/gtfkwworpq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gtdrumthnb.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtdipdvvmx.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.xuetiantiany.cn/gtfmypxhph.html

[U84] JS：CommonJS 写法
来源：http://hz.smart0.xyz/gtjizkqjku.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.daria6918.cn/gtvmenyhrx.html

[U85] JS：可选链
来源：http://hz.gzhubu.top/gtjuukbwrk.html

a?.b?.c
来源：http://hz.snrcjt.cn/gtrrnkpspo.html

[U86] JS：空值合并
来源：http://hz.hnqzz.top/gttqpucpwu.html

a ?? b
来源：http://hz.xinyue.icu/gtjlqwztes.html

[U87] JS：解构默认值
来源：http://hz.hnxiangtu.top/gtpkygutjh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xuetiantiany.cn/gtsnvigtsl.html

[U88] JS：对象展开合并
来源：http://hz.shanyushiyangkeji.top/gtddwrutuv.html

{ ...a, ...b }
来源：http://hz.cheryme.top/gtltbkydvr.html

[U89] JS：数组去重
来源：http://hz.gaohongyu789.top/gtjclolcbo.html

[...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtnfbwyfpy.html

[U90] JS：数字数组排序
来源：http://hz.xylfe.cn/gtirnyrqkc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtpjuhvvoj.html

[U91] JS：对象键值遍历
来源：http://hz.ppjwa.cn/gtelpdyvuy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.9152youxi.cn/gtgmalvuxh.html

[U92] JS：深拷贝
来源：http://hz.dianchejie.cn/gtdhzlzcsa.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gtehprkyux.html

[U93] JS：模板字符串
来源：http://hz.yueranfly.top/gtzlpgtris.html

`共 ${n} 条`
来源：http://hz.cucudq.cn/gtdattarwj.html

[U94] JS：箭头函数
来源：http://hz.yanxiufei.cn/gtpmrikeus.html

const double = x => x * 2;
来源：http://hz.nanxinkj.top/gtomgoivgu.html

[U95] JS：Promise 包装
来源：http://hz.pycfn.com/gtknvurzup.html

new Promise((resolve, reject) => {})
来源：http://hz.cdnleiting.top/gtkedsvawu.html

[U96] JS：async/await 与异常
来源：http://hz.gzhubu.top/gttgpruhgk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtlcubqhbr.html

[U97] JS：并发请求
来源：http://hz.zhijiandao.cn/gtankwibfz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtkioqddvb.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhiwuduotai.top/gtsjehirrg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ydzc1.top/gtshbdmcyc.html

[U99] JS：事件监听
来源：http://hz.iojbl.cn/gtukucbsaa.html

el.addEventListener("click", e => {})
来源：http://hz.daxiang520.top/gtkampzuuy.html

[U100] JS：DOM 查询
来源：http://hz.jqgfzy.top/gtbkydgqlj.html

document.querySelector(".item")
来源：http://hz.hnqzz.top/gticzagtas.html

[U101] JS：classList 操作
来源：http://hz.sweek.top/gtwumtxmgy.html

el.classList.toggle("active")
来源：http://hz.zhixingplan.top/gtiwmqrwkv.html

[U102] JS：本地存储
来源：http://hz.zycfv.cn/gtofwdmktf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jinqigfzy.top/gtarfcwvjj.html

[U103] JS：定时器
来源：http://hz.0kj1m.cn/gtqctguvaf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hfpthk.cn/gtmifpwmtm.html

[U104] JS：防抖
来源：http://hz.gotoacloud.top/gthjpschxx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtkxmosjvr.html

[U105] JS：节流
来源：http://hz.sysykeji.top/gtebtvetcz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtjbvhlrjs.html

[U106] JS：日期格式化
来源：http://hz.birdmap.top/gttxgbhxgm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hysaishi.cn/gtsujafpaj.html

[U107] JS：数字千分位
来源：http://hz.yj202588.top/gtmweugpys.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aibaodan.cn/gtvwncnuji.html

[U108] JS：随机整数
来源：http://hz.wangdashe.top/gtxpubimkp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtsxssgixx.html

[U109] JS：数组分组
来源：http://hz.fzhhl.top/gtmnyzhlws.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenlongwang.top/gtejewxvke.html

[U110] JS：数组分块
来源：http://hz.jinghuilouyu.cn/gtizchijse.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258888.top/gtfbzakcqx.html

[U111] JS：对象转 Map
来源：http://hz.cheryme.top/gtfbxtnked.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtpqmeqdxs.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gtstwsogqw.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtfygjwfme.html

[U113] JS：正则替换全部
来源：http://hz.jinghuilouyu.cn/gtrqbdednm.html

s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtqaycbups.html

[U114] JS：JSON 深比较
来源：http://hz.jinyuanbaomall.cn/gtyyxytrdz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.iojbl.cn/gtwjeakinn.html

[U115] JS：生成 UUID
来源：http://hz.guannengcc.top/gtmgtadtcf.html

crypto.randomUUID()
来源：http://hz.bjfxy.top/gtqgydjfuv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhiwuduotai.top/gtjdwcnmvh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zdqjudy.top/gtqzufjtqq.html

[U117] JS：单元测试
来源：http://hz.dianchejie.cn/gtseebumnb.html

npm i -D vitest;  npx vitest
来源：http://hz.jqgufenzy.top/gtptjgrjpe.html

[U118] JS：开发服务器
来源：http://hz.yueranfly.top/gtqtcidrvx.html

npm i -D vite;  npx vite
来源：http://hz.gaohongyu789.top/gtidgqgbps.html

[U119] JS：生产构建
来源：http://hz.hammf.cn/gtrujfseuy.html

npx vite build
来源：http://hz.0kj1m.cn/gtwuhcckoc.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sufxvd.cn/gtrsfsuxnj.html

import.meta.env.VITE_API_URL
来源：http://hz.sweek.top/gteeyijmbr.html

================================================================================
来源：http://hz.zhengqikj.top/gtxbcqiyil.html

统计汇总
来源：http://hz.daxiang520.top/gtrlpigvkv.html

================================================================================
来源：http://hz.cashguo.top/gtdebwgpkp.html

按语言统计（条）：
来源：http://hz.jyoumei.cn/gtxldpysyd.html

Python ......... 252
来源：http://hz.svipenyu.cn/gtuyexwyqb.html

PHP ............ 252
来源：http://hz.dianchejie.cn/gtgdkawvet.html

JavaScript ..... 252
来源：http://hz.shuidangran.top/gticiexvyr.html

TypeScript ..... 212
来源：http://hz.xziqi.cn/gtqzullpuu.html

Java ........... 212
来源：http://hz.tian-w.cn/gtdfuyocxo.html

Go ............. 212
来源：http://hz.bjfxy.top/gtuqpnrqus.html

Ruby ........... 212
来源：http://hz.cdnleiting.top/gtcqelhhxu.html

C# ............. 212
来源：http://hz.xziqi.cn/gtkzayyxdk.html

C .............. 30
来源：http://hz.zhoulong.xyz/gtskihbxqj.html

C++ ............ 30
来源：http://hz.jlsjyb.cn/gtvpdkkrna.html

SQL ............ 90
来源：http://hz.hammf.cn/gtmquhqzus.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtispouwsf.html

Kotlin ......... 15
来源：http://hz.sufxvd.cn/gtxcbtjhpv.html

Swift .......... 15
来源：http://hz.jiagoushi.top/gtaqnaczje.html

Lua ............ 10
来源：http://hz.chenzaomai.com/gtminvipas.html

Perl ........... 10
来源：http://hz.birdmap.top/gtnixxkmdx.html

Scala .......... 10
来源：http://hz.shuidangran.top/gtlynnenfe.html

------------------------------------
来源：http://hz.zhijiandao.cn/gtjdhqhvne.html

合计 ........... 2106 条
来源：http://hz.xuetiantiany.cn/gtwnfzquvt.html

按章节统计：
来源：http://hz.xinyue.icu/gtgprwpntw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gteqgawyaw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtcinbfbiv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtczlcrhsl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtahjtdbaq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xingfuxueyuan.xyz/gticwicnje.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtqraqadev.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtmnrwmvhj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ivvv.top/gtzstbpmkj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtdelizmyx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinqigufen.top/gtueppnhez.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtwxgtkods.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gttzkrolha.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtwixusuvm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gthppqyncq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gtdmnamiwu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtcnsonwyx.html

Q SQL 专题                              90
来源：http://hz.hongshengwenyu.top/gtrspkctxm.html

R Bash 专题                             80
来源：http://hz.tanke756.top/gtzppnupcm.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtcdhheabx.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtsiyrpvhk.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtzucowowh.html

------------------------------------
来源：http://hz.hnxiangtu.top/gtgloljeak.html

合计                                  2106 条
来源：http://hz.shanyushiyangtech.top/gtsfwslsje.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtnzjfobnl.html

使用提醒
来源：http://hz.0kj1m.cn/gtxynurqjv.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtjesdrkvk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.feifeiyinyue.top/gtijgvvmdz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnxiangtu.top/gtkhoncsov.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fzhhl.top/gtkhxouhvl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.guowangkeji.top/gtyqrlqlxa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.gzhubu.top/gthaolzmkn.html

—— 文件结束 ——
来源：http://hz.yvedp.cn/gtuxesmdtb.html

================================================================================
来源：http://hz.c1oappe.top/gtydjctkmm.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.dianchejie.cn/gtqkosiyni.html

Common Programming Examples Cheat Book
来源：http://hz.hnxiangtu.top/gtjyowcywz.html

================================================================================
来源：http://hz.smart0.xyz/gtxjbzalxa.html

【收录内容】
来源：http://hz.sysykeji.top/gtcwnnexve.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtxvcsyesw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tianlin.xyz/gttuilgvfc.html

SQL · Bash · C · C++
来源：http://hz.smart0.xyz/gtrfazokbq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gogol.net.cn/gtvgduoprn.html

【使用说明】
来源：http://hz.gotoacloud.top/gtjbrvsmkp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hfpthk.cn/gtddywhbzb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zdqjudy.top/gtllipjznx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.aizwys.cn/gtckjkfejc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenlongwang.top/gtcmkwpzpy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nanxinkj.top/gttenmjroa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xinyue.icu/gtykmqyfjy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.0kj1m.cn/gtpmiipdrs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.chenlongwang.top/gtxfkgrqyn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sweek.top/gtjllmbqlf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yj20258.top/gtikjlzbbn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnqzz.top/gtjuduxyfc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zdqjudy.top/gtfjiqizty.html

【文件统计】
来源：http://hz.zhiwuduotai.top/gtexqgoajp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj20258888.top/gtsnppgxvr.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtucwfpduy.html

目  录
来源：http://hz.gotoacloud.top/gtdffhawks.html

--------------------------------------------------------------------------------
来源：http://hz.sysykeji.top/gteoctxzgs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.havefunace.top/gtbqbssdil.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gttopftrfk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtqshjkmrw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.gogol.net.cn/gtjgsofjke.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pengpengdd.cyou/gttjrtsweg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinghuilouyu.cn/gtbfsywvbz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtbpwwjbol.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.gotoacloud.top/gtpcitvcpq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gttimdalob.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yj202588.top/gtpbkewxsq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtnqazqrjz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cdnleiting.top/gtozdgonlv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtafsxhjbd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtumnxtqye.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yj202588.top/gtqrgyjudn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtjhvwfeyz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtupdpncjd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.dashuyun.cn/gtvcipkuin.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nwbrower.top/gtplqiukck.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gtnftgrzmj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtwegehhrz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxppuqhna.html

A. 基础语法与类型
来源：http://hz.yangfankeji.com/gtuqdudcjr.html

================================================================================
来源：http://hz.daxiang520.top/gtcussmlvf.html

[A01] Hello World
来源：http://hz.zhaomingkeji.xyz/gtxvzvirqn.html

Py:   print("Hello, World!")
来源：http://hz.mhx1999.top/gtzbcwfapl.html

PHP:  echo "Hello, World!";
来源：http://hz.ydjk.org.cn/gtennqsqpk.html

JS:   console.log("Hello, World!");
来源：http://hz.zhengqikj.top/gtvurdmxor.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cqqwz.cn/gtxfmvifox.html

Java: System.out.println("Hello, World!");
来源：http://hz.guannengcc.top/gttjdmyudn.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.0kj1m.cn/gtinsfrryh.html

Ruby: puts "Hello, World!"
来源：http://hz.xinyue.icu/gtnjtmirse.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhongyouzk.top/gtpcedcppu.html

[A02] 变量声明与赋值
来源：http://hz.dianchejie.cn/gthlgwjila.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jiagoushi.top/gthrbopjyf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtfadqiynt.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jinghuilouyu.cn/gtkdiubeyl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ybcxt.top/gtsvxoivrw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.gzhubu.top/gtleftvhzr.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangdashe.top/gtmngplnll.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhixingplan.top/gtxquesjcm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.xziqi.cn/gtgfizfbcf.html

[A03] 常量定义
来源：http://hz.nanxinkj.top/gtvqgcranv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yonumen.top/gthjvkcumi.html

PHP:  const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtnimtbzso.html

JS:   const PI = 3.14159;
来源：http://hz.0kj1m.cn/gtdjbcsuuu.html

TS:   const PI: number = 3.14159;
来源：http://hz.fzhhl.top/gtiunwhois.html

Java: static final double PI = 3.14159;
来源：http://hz.ydjk.org.cn/gtcenfcyvi.html

Go:   const PI = 3.14159
来源：http://hz.jiagoushi.top/gtvkwvysxk.html

Ruby: PI = 3.14159
来源：http://hz.cdnleiting.top/gtrkrejsho.html

C#:   const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtryvqfeyn.html

[A04] 判断变量类型
来源：http://hz.fengsongda.top/gttnddrsdm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.andypj.xyz/gtbxtpsozf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.aibaodan.cn/gtsugosyqw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.haohaochexian.top/gtyegyvxis.html

TS:   typeof x; x instanceof Date
来源：http://hz.yangfankeji.com/gtvhsqhhtp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gzhubu.top/gtpmpootdc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.sxryk.cn/gtetnpuide.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xziqi.cn/gtnvmyyfom.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtvbmdcdzc.html

[A05] 整数除法与取模
来源：http://hz.yj20258888.top/gtaeljkunq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ivvv.top/gtnjcftjqs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.shzxlz.cn/gthbperisw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sxryk.cn/gtepeggkqt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zdqjudy.top/gtfvhaxprf.html

Java: 7 / 2; 7 % 2
来源：http://hz.pengpengdd.cyou/gtvtgbeuna.html

Go:   7 / 2; 7 % 2
来源：http://hz.hnqzz.top/gtaodkxbmp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jianghu66.top/gtemysbswa.html

C#:   7 / 2; 7 % 2
来源：http://hz.cashguo.top/gtvoqmflqj.html

[A06] 字符串转数字
来源：http://hz.nanxinkj.top/gtlniysfzo.html

Py:   int("42"); float("3.14")
来源：http://hz.fengsongda.top/gtwitgmzny.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ivvv.top/gtyguflpgl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sysykeji.top/gtgbdjpsbn.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.wangshuangyany.cn/gtohdkjxmm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hammf.cn/gtmxgwmjxo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.andypj.xyz/gtyimndqyo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yj202588.top/gtqnjvmkvu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.9152youxi.cn/gtmdyighve.html

[A07] 数字转字符串
来源：http://hz.hnxiangtu.top/gtiptvvnro.html

Py:   str(42)
来源：http://hz.daxiang520.top/gtbfzvsakr.html

PHP:  (string) 42; strval(42)
来源：http://hz.yuanzhike.top/gtrookknto.html


<!-- 参考信息 -->