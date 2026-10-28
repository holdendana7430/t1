代发 wailian999

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtwukpgkcp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shangyingyoupin.top/gtswlohjct.html

[U60] PHP：JSON 编解码
来源：http://hz.mhx1999.top/gtbxdlpgyj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.0kj1m.cn/gtebrznjjo.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gtnxvjfjws.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtanbwmcok.html

[U62] PHP：日期对象
来源：http://hz.gzhubu.top/gthuywvtgq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.daxiang520.top/gtwgvnmoho.html

[U63] PHP：文件读写
来源：http://hz.xinyue.icu/gtzyxjftvo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xylfe.cn/gtosjperii.html

[U64] PHP：目录遍历
来源：http://hz.yuanzhike.top/gtzykinfic.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.svipenyu.cn/gtkxzkyxjr.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gtkbypvgtm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cdnleiting.top/gtfhxhtrne.html

[U66] PHP：设置 Cookie
来源：http://hz.c1oappe.top/gtboriyopo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hnxiangtu.top/gtskhymjwm.html

[U67] PHP：处理文件上传
来源：http://hz.meibo888.top/gtbosbdbgw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xinyue.icu/gtnvlxqpyo.html

[U68] PHP：PDO 连接
来源：http://hz.zhengqikj.top/gtctgjkooe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.iojbl.cn/gtltfbzvjd.html

[U69] PHP：PDO 预处理
来源：http://hz.ydjk.org.cn/gtbtznhken.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hnxiangtu.top/gtkunmfsif.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtsqugveva.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shanyushiyangkeji.top/gtxgadvlli.html

[U71] PHP：抛出异常
来源：http://hz.sufxvd.cn/gtgczkoqhl.html

throw new RuntimeException("失败", 500);
来源：http://hz.cdnleiting.top/gttuiusuzc.html

[U72] PHP：写错误日志
来源：http://hz.snrcjt.cn/gtcjoaooxi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xingfuxueyuan.xyz/gtuojvshtr.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinghuilouyu.cn/gtjajklckb.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gthcfietpm.html

[U74] PHP：读取环境变量
来源：http://hz.pengpengdd.cyou/gtjsljxbvw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dashuyun.cn/gtdsowsdnz.html

[U75] PHP：依赖注入
来源：http://hz.zhengqikj.top/gtfzxesafc.html

composer require psr/container
来源：http://hz.xingfuxueyuan.xyz/gtppcbdqkj.html

[U76] PHP：简单路由
来源：http://hz.daria6918.cn/gtiahrvcka.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zdqjudy.top/gtbkhvyqkc.html

[U77] PHP：模板渲染
来源：http://hz.yangfankeji.com/gtqfowsgnj.html

composer require twig/twig
来源：http://hz.sweek.top/gtnfagnxbf.html

[U78] PHP：单元测试
来源：http://hz.nwbrower.top/gtjxdsmkeo.html

composer require --dev phpunit/phpunit
来源：http://hz.sysykeji.top/gtyetsngli.html

[U79] PHP：静态分析
来源：http://hz.ydzc1.top/gtptgsbdez.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgufenzy.top/gtkzezomjo.html

[U80] PHP：代码规范修复
来源：http://hz.hongshengwenyu.top/gttdqqaorc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gtpwwtdgva.html

[U81] JS：初始化项目
来源：http://hz.shuidangran.top/gtunfcrnqv.html

npm init -y;  npm i express
来源：http://hz.sysykeji.top/gtinolggyq.html

[U82] JS：package.json 脚本
来源：http://hz.chenjidiqi.icu/gtskpdxyxb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.birdmap.top/gtqtvvpymi.html

[U83] JS：ES Module 导入导出
来源：http://hz.redwolf501.top/gthspyqqoq.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtbtnllnrf.html

[U84] JS：CommonJS 写法
来源：http://hz.zhijiandao.cn/gtaanazhlm.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhaomingkeji.xyz/gtgjcdwecb.html

[U85] JS：可选链
来源：http://hz.redwolf501.top/gtefsqvyjd.html

a?.b?.c
来源：http://hz.jqgfzy.top/gtpauejjwe.html

[U86] JS：空值合并
来源：http://hz.daxiang520.top/gtgydrlugk.html

a ?? b
来源：http://hz.hfpthk.cn/gtmlmuvkbq.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtahojjxba.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gogol.net.cn/gtxhqyhneu.html

[U88] JS：对象展开合并
来源：http://hz.jqgfzy.top/gtlomaokrn.html

{ ...a, ...b }
来源：http://hz.tian-w.cn/gtaafzptkl.html

[U89] JS：数组去重
来源：http://hz.pengpengdd.cyou/gtqjdsslam.html

[...new Set(arr)]
来源：http://hz.ydzc1.top/gtbpuwztef.html

[U90] JS：数字数组排序
来源：http://hz.nwbrower.top/gtuswwgvfd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtkdzeklpg.html

[U91] JS：对象键值遍历
来源：http://hz.sysykeji.top/gtxwrwsmjt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yvedp.cn/gttrtdtpfy.html

[U92] JS：深拷贝
来源：http://hz.zhijiandao.cn/gthgmxlbrh.html

structuredClone(obj)
来源：http://hz.aibaodan.cn/gthdmkgfju.html

[U93] JS：模板字符串
来源：http://hz.quarkkingdee.top/gtuktskzqq.html

`共 ${n} 条`
来源：http://hz.yuanzhike.top/gtsluusnce.html

[U94] JS：箭头函数
来源：http://hz.aibaodan.cn/gtxahasevo.html

const double = x => x * 2;
来源：http://hz.snrcjt.cn/gtqjaeqbxp.html

[U95] JS：Promise 包装
来源：http://hz.c1oappe.top/gtmtlawfxi.html

new Promise((resolve, reject) => {})
来源：http://hz.hywenlv.cn/gtlkegnzzy.html

[U96] JS：async/await 与异常
来源：http://hz.yanxiufei.cn/gtkywkurhw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtguukkgym.html

[U97] JS：并发请求
来源：http://hz.havefunace.top/gtjlbbbyxv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtzkoeykje.html

[U98] JS：fetch 带 JSON
来源：http://hz.daria6918.cn/gtxwwuouzg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinqigfzy.top/gteypdnsoh.html

[U99] JS：事件监听
来源：http://hz.bjfxy.top/gtslyaurzc.html

el.addEventListener("click", e => {})
来源：http://hz.havefunace.top/gtfgczucnp.html

[U100] JS：DOM 查询
来源：http://hz.snrcjt.cn/gtwjswmrut.html

document.querySelector(".item")
来源：http://hz.bjfxy.top/gtaxxsbbyd.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtcvvabsmr.html

el.classList.toggle("active")
来源：http://hz.bjfxy.top/gtrkjpuldb.html

[U102] JS：本地存储
来源：http://hz.316326.xyz/gtcahezery.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hammf.cn/gtthcorefa.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtavhwftwm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenlongwang.top/gtlrutrozc.html

[U104] JS：防抖
来源：http://hz.jianghu66.top/gtwqajzjct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhengqikj.top/gtxhsjoixu.html

[U105] JS：节流
来源：http://hz.jinghuilouyu.cn/gtktytkggm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhengqikj.top/gtecsikhov.html

[U106] JS：日期格式化
来源：http://hz.quarkkingdee.top/gttfadcxpo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhongyouzk.top/gtloshrpne.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gtpmayopge.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhongyouzk.top/gtjbnzwpsv.html

[U108] JS：随机整数
来源：http://hz.c1oappe.top/gtivlyayfi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.chenlongwang.top/gthqepenfy.html

[U109] JS：数组分组
来源：http://hz.sysykeji.top/gtuyzkatac.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtreuadztb.html

[U110] JS：数组分块
来源：http://hz.yuanzhike.top/gttnauxnqt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnqzz.top/gtfthyfcdk.html

[U111] JS：对象转 Map
来源：http://hz.jyoumei.cn/gttbvgjzmg.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtbwdefffs.html

[U112] JS：字符串补位
来源：http://hz.fengsongda.top/gtqodwammv.html

"7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtdhevhzjo.html

[U113] JS：正则替换全部
来源：http://hz.sweek.top/gtmapxbedd.html

s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtxtfytxmv.html

[U114] JS：JSON 深比较
来源：http://hz.fzhhl.top/gtagycfhqt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtknjdeitb.html

[U115] JS：生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtlnypmkis.html

crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtwejfktqq.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xylfe.cn/gtmyobcelp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yanxiufei.cn/gtbnqegiiv.html

[U117] JS：单元测试
来源：http://hz.ppjwa.cn/gtqngclkte.html

npm i -D vitest;  npx vitest
来源：http://hz.sufxvd.cn/gttctqalxa.html

[U118] JS：开发服务器
来源：http://hz.chenzaomai.com/gtkkizgkda.html

npm i -D vite;  npx vite
来源：http://hz.cdnleiting.top/gtmcakrrjn.html

[U119] JS：生产构建
来源：http://hz.yuanzhike.top/gtnyaqmxdo.html

npx vite build
来源：http://hz.gogol.net.cn/gthgnalsoq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtbfhwjomn.html

import.meta.env.VITE_API_URL
来源：http://hz.sysykeji.top/gtjvartuut.html

================================================================================
来源：http://hz.yuanzhike.top/gtqmabeeni.html

统计汇总
来源：http://hz.yangfankeji.com/gtdukiqjwc.html

================================================================================
来源：http://hz.cucudq.cn/gtmufrjgdw.html

按语言统计（条）：
来源：http://hz.ehwqpu.com/gtnuvprool.html

Python ......... 252
来源：http://hz.iojbl.cn/gtuklwukhs.html

PHP ............ 252
来源：http://hz.jinqigufen.top/gtbolzlghq.html

JavaScript ..... 252
来源：http://hz.hammf.cn/gtyuqpmuby.html

TypeScript ..... 212
来源：http://hz.jianghu66.top/gtchrucsll.html

Java ........... 212
来源：http://hz.aizwys.cn/gttgtsfreo.html

Go ............. 212
来源：http://hz.xylfe.cn/gtshbfzzpf.html

Ruby ........... 212
来源：http://hz.ywan-chungtsiang.top/gtasxnutrx.html

C# ............. 212
来源：http://hz.zhijiandao.cn/gtyenafmhj.html

C .............. 30
来源：http://hz.zhengqikj.top/gtptnhmdfj.html

C++ ............ 30
来源：http://hz.sysykeji.top/gtsimzmuhd.html

SQL ............ 90
来源：http://hz.sxryk.cn/gtuhmcaeqr.html

Bash ........... 80
来源：http://hz.tianlin.xyz/gtlgoplufe.html

Kotlin ......... 15
来源：http://hz.sufxvd.cn/gtfuwzctjj.html

Swift .......... 15
来源：http://hz.iojbl.cn/gtenxjgmaj.html

Lua ............ 10
来源：http://hz.dianchejie.cn/gtvqvzdiai.html

Perl ........... 10
来源：http://hz.ppjwa.cn/gtkkbubuld.html

Scala .......... 10
来源：http://hz.havefunace.top/gtjgwctntr.html

------------------------------------
来源：http://hz.meibo888.top/gthfrnusdu.html

合计 ........... 2106 条
来源：http://hz.yj202588.top/gtrwmrhgmv.html

按章节统计：
来源：http://hz.jyoumei.cn/gtxylcqusu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinghuilouyu.cn/gtpzonvzfy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.316326.xyz/gtdnngimwv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtqglwovvl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtskssitsa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtlbbdtxyj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.vqdsnc.cn/gtqvdtqrxl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtotvwwklj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shzxlz.cn/gtvkcvxnuk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtanmznbfa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtvdeqiera.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtcsseohod.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtzsptyzzf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtescbcuzm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.meibo888.top/gtsstssnaa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtanyupnji.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtxazpisyl.html

Q SQL 专题                              90
来源：http://hz.0kj1m.cn/gtscujitda.html

R Bash 专题                             80
来源：http://hz.cashguo.top/gtmtwusyyh.html

S C / C++ 专题                          60
来源：http://hz.jianghu66.top/gtxfbrtmse.html

T 其他语言补充                          60
来源：http://hz.zhoulong.xyz/gtbqewejcx.html

U 高频实用片段                         120
来源：http://hz.xylfe.cn/gtultkkqtg.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtehgpgsdp.html

合计                                  2106 条
来源：http://hz.vqdsnc.cn/gtzyoreior.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtmchvivij.html

使用提醒
来源：http://hz.bjfxy.top/gtzhyxekub.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtovjrblso.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.xuanzx.com/gtdbqvrgpe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fengsongda.top/gtpxiqpwio.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.dashuyun.cn/gtydbuohot.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhongyouzk.top/gtxmkmtgqi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.snrcjt.cn/gtbvykozlo.html

—— 文件结束 ——
来源：http://hz.hnqzz.top/gtzthovjrg.html

================================================================================
来源：http://hz.cqqwz.cn/gtyjpvuwaw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cashguo.top/gteoqyfmpx.html

Common Programming Examples Cheat Book
来源：http://hz.cqqwz.cn/gtkgruepcz.html

================================================================================
来源：http://hz.hfpthk.cn/gtrhjdkoju.html

【收录内容】
来源：http://hz.aizwys.cn/gtwuuuoipn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.nwbrower.top/gtmswfetjc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhoulong.xyz/gtesktvdte.html

SQL · Bash · C · C++
来源：http://hz.jinyuanbaomall.cn/gtifuxybjv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhixingplan.top/gtiuofnsos.html

【使用说明】
来源：http://hz.cqqwz.cn/gthlbsljeb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.tian-w.cn/gtfhzsmaht.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhijiandao.cn/gtaovidbrk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.tianlin.xyz/gtraacsjma.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yangfankeji.com/gtijcgrpqt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ivvv.top/gtlnttvzmp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ivvv.top/gtexcrzets.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnqzz.top/gtrrtevpox.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.birdmap.top/gtprccklrk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.chenlongwang.top/gtlzazvstq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tian-w.cn/gtqgtulvnk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.birdmap.top/gtyylnqnin.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinyuanbaomall.cn/gtsnqqptaa.html

【文件统计】
来源：http://hz.quarkkingdee.top/gtowhchmuz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhongyouzk.top/gtgvuhrdfu.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtaxatbwqy.html

目  录
来源：http://hz.cdnleiting.top/gtluegsvir.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gtkuifgpnh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gtaocjbabc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtwkyddtxr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cashguo.top/gtpkosnkvj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gtxeycmvhm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxinkj.top/gtaezshhhk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.tanke756.top/gtkbgcfsdy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtcemmikko.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.birdmap.top/gtlbpocdqt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtkisqizoy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yonumen.top/gtqtjamiiz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gttimxpjtg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtpuiirbvz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.mhx1999.top/gtqozfjpma.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtwtesgoul.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sufxvd.cn/gtizbxbxad.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtnrtxlfce.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gotoacloud.top/gtdqopbxdq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.mhx1999.top/gtpetmdver.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.andypj.xyz/gtujpzkfuw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtmtlovtgo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gttzefklqc.html

================================================================================
来源：http://hz.tian-w.cn/gtqjbqjvqo.html

A. 基础语法与类型
来源：http://hz.zhengqikj.top/gtkzrzqkez.html

================================================================================
来源：http://hz.cashguo.top/gtonqzjlcv.html

[A01] Hello World
来源：http://hz.52xcode.cn/gtxcqtwhxw.html

Py:   print("Hello, World!")
来源：http://hz.gzhubu.top/gtmsgunkex.html

PHP:  echo "Hello, World!";
来源：http://hz.iojbl.cn/gtwbmxwmrl.html

JS:   console.log("Hello, World!");
来源：http://hz.xylfe.cn/gtkoufwhzm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.wangshuangyany.cn/gtoaiazoyv.html

Java: System.out.println("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtbqnvssra.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtbfnntsvh.html

Ruby: puts "Hello, World!"
来源：http://hz.ydjk.org.cn/gtyxzxnasp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hnxiangtu.top/gtwzhwgajx.html

[A02] 变量声明与赋值
来源：http://hz.jianghu66.top/gtravkoxwi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.pycfn.com/gtwglxyzhh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aibaodan.cn/gtslpyzkwk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.havefunace.top/gtdklajiki.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jqgufenzy.top/gtsqrjoayp.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.daria6918.cn/gtbviiqvxn.html

Go:   name := "Alex"; age := 20
来源：http://hz.sufxvd.cn/gtjzzmfyiw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.chenlongwang.top/gtemqqirap.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinghuilouyu.cn/gtutxuzvlp.html

[A03] 常量定义
来源：http://hz.guowangkeji.top/gtvbenfavi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jlsjyb.cn/gtrlwjevdr.html

PHP:  const PI = 3.14159;
来源：http://hz.feifeiyinyue.top/gtigctbvun.html

JS:   const PI = 3.14159;
来源：http://hz.aibaodan.cn/gtrgghsuun.html

TS:   const PI: number = 3.14159;
来源：http://hz.yongpay.top/gtfxzkwjir.html

Java: static final double PI = 3.14159;
来源：http://hz.ybcxt.top/gtputjkxqz.html

Go:   const PI = 3.14159
来源：http://hz.xuetiantiany.cn/gtmszddsob.html

Ruby: PI = 3.14159
来源：http://hz.hfpthk.cn/gtcqnmfqwn.html

C#:   const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtenbwlsch.html

[A04] 判断变量类型
来源：http://hz.quarkkingdee.top/gtalpzwmwf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.fengsongda.top/gtntlbevkf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.haohaochexian.top/gtzttehize.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.cashguo.top/gttozsbhhh.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangdashe.top/gtfskpvnpd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ehwqpu.com/gtrestkbhy.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shzxlz.cn/gtvqfpaqei.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.316326.xyz/gtzemxnhga.html

C#:   x.GetType().Name; x is int
来源：http://hz.sxryk.cn/gtewpziuon.html

[A05] 整数除法与取模
来源：http://hz.meibo888.top/gtbzdwhijm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.9152youxi.cn/gtfkzeudux.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.redwolf501.top/gtwceitzfr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtuahhbbbt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtypifrvug.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtjjwbunoa.html

Go:   7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtorwotras.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtvuldiycc.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtpwcjaxbu.html

[A06] 字符串转数字
来源：http://hz.zhengqikj.top/gtayvkbqtq.html

Py:   int("42"); float("3.14")
来源：http://hz.aibaodan.cn/gtrmfuhvlr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yongpay.top/gtbdnydnra.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ybcxt.top/gtittvvilw.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zdqjudy.top/gtrqxcewgd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hysaishi.cn/gtceezwsym.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cdnleiting.top/gtwojjfrjp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.fengsongda.top/gtmztuktgj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jiagoushi.top/gtbsuwrrjj.html

[A07] 数字转字符串
来源：http://hz.shangyingyoupin.top/gtsbstojds.html

Py:   str(42)
来源：http://hz.jianghu66.top/gtfkmyvavj.html

PHP:  (string) 42; strval(42)
来源：http://hz.jinqigfzy.top/gtydtuoqpr.html

JS:   String(42); (42).toString()
来源：http://hz.gzhubu.top/gtnpbzzcob.html

TS:   String(42)
来源：http://hz.cucudq.cn/gtcyzlfkuj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ehwqpu.com/gtgelhgoyk.html

Go:   strconv.Itoa(42)
来源：http://hz.ivvv.top/gtkneuwken.html

Ruby: 42.to_s
来源：http://hz.gotoacloud.top/gtvgpyplik.html

C#:   42.ToString()
来源：http://hz.xinyue.icu/gtqhokqrsf.html

[A08] 取整与四舍五入
来源：http://hz.shangyingyoupin.top/gtyaqpczxm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.gzhubu.top/gtapecpvft.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.guannengcc.top/gtuzjaucbb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.snrcjt.cn/gtglykufds.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.kuanghao11.cn/gttekhtwyf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jianghu66.top/gtfcdllxii.html


<!-- 参考信息 -->