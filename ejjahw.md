代发 wailian999

[U61] PHP：正则
来源：http://hz.9152youxi.cn/gtcjatsdst.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtqejyiyyq.html

[U62] PHP：日期对象
来源：http://hz.fengsongda.top/gthrctinlx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gtmqtktslp.html

[U63] PHP：文件读写
来源：http://hz.shuidangran.top/gtltjryosh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xingfuxueyuan.xyz/gtmfvbkavt.html

[U64] PHP：目录遍历
来源：http://hz.ivvv.top/gtfffmfpbf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj202588.top/gtrzvhgcjt.html

[U65] PHP：会话
来源：http://hz.zhaomingkeji.xyz/gtzvlbezhm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydzc1.top/gtldcoihwt.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtmemwwmtz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.daria6918.cn/gtqtmzexgx.html

[U67] PHP：处理文件上传
来源：http://hz.quarkkingdee.top/gtdyfdfqqt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aibaodan.cn/gtmysvtrdh.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtnfddjzws.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ppjwa.cn/gtavagaqho.html

[U69] PHP：PDO 预处理
来源：http://hz.yj202588.top/gtffymtywt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.vqdsnc.cn/gtezhnbdpe.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gthepgqfpe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgufenzy.top/gtbsdiacpw.html

[U71] PHP：抛出异常
来源：http://hz.xuetiantiany.cn/gthplsvfxb.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuetiantiany.cn/gtrziiagjs.html

[U72] PHP：写错误日志
来源：http://hz.redwolf501.top/gtpevjjoxu.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hammf.cn/gthfycvcms.html

[U73] PHP：读取 ini 配置
来源：http://hz.dashuyun.cn/gttyeaftet.html

parse_ini_file("config.ini", true)
来源：http://hz.mhx1999.top/gtkqvykisf.html

[U74] PHP：读取环境变量
来源：http://hz.andypj.xyz/gtlhvcuqau.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtdvqmdape.html

[U75] PHP：依赖注入
来源：http://hz.cqqwz.cn/gtipirycif.html

composer require psr/container
来源：http://hz.ehwqpu.com/gtknsokald.html

[U76] PHP：简单路由
来源：http://hz.havefunace.top/gtmeiyeemm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxinkj.top/gtzajkwtlh.html

[U77] PHP：模板渲染
来源：http://hz.daxiang520.top/gtvuerfabt.html

composer require twig/twig
来源：http://hz.shanyushiyangtech.top/gtppjsixnv.html

[U78] PHP：单元测试
来源：http://hz.yangfankeji.com/gtukklyihk.html

composer require --dev phpunit/phpunit
来源：http://hz.316326.xyz/gtowngyyiw.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtqkesvhsn.html

composer require --dev phpstan/phpstan
来源：http://hz.tianlin.xyz/gttjegadvz.html

[U80] PHP：代码规范修复
来源：http://hz.cqqwz.cn/gtoykhdyka.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pycfn.com/gtfohvnspq.html

[U81] JS：初始化项目
来源：http://hz.c1oappe.top/gtmewsqcoe.html

npm init -y;  npm i express
来源：http://hz.jinyuanbaomall.cn/gticmqancs.html

[U82] JS：package.json 脚本
来源：http://hz.guannengcc.top/gtkefqzgtm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhixingplan.top/gtfefeaamw.html

[U83] JS：ES Module 导入导出
来源：http://hz.andypj.xyz/gthlcmwmgp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.smart0.xyz/gtprheyizc.html

[U84] JS：CommonJS 写法
来源：http://hz.jlsjyb.cn/gtrkacannj.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shanyushiyangtech.top/gtbjswdvxz.html

[U85] JS：可选链
来源：http://hz.sxryk.cn/gtiktrjlcw.html

a?.b?.c
来源：http://hz.shzxlz.cn/gtvnvedppa.html

[U86] JS：空值合并
来源：http://hz.xziqi.cn/gtcagkwwpb.html

a ?? b
来源：http://hz.yonumen.top/gttgypfblz.html

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtdspycudd.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jlsjyb.cn/gthqsjuuek.html

[U88] JS：对象展开合并
来源：http://hz.ppjwa.cn/gtqwgliolp.html

{ ...a, ...b }
来源：http://hz.sufxvd.cn/gtofmugasr.html

[U89] JS：数组去重
来源：http://hz.shangyingyoupin.top/gtfptwavah.html

[...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtvubuyijm.html

[U90] JS：数字数组排序
来源：http://hz.shanyushiyangtech.top/gtytuyntnz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtqjuwvmqx.html

[U91] JS：对象键值遍历
来源：http://hz.jlsjyb.cn/gtxxgpplmj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jianghu66.top/gttjyffvqj.html

[U92] JS：深拷贝
来源：http://hz.tanke756.top/gtbsczvfmk.html

structuredClone(obj)
来源：http://hz.tianlin.xyz/gtqredndxs.html

[U93] JS：模板字符串
来源：http://hz.wangdashe.top/gtawltpywv.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtweqdmlnd.html

[U94] JS：箭头函数
来源：http://hz.gotoacloud.top/gtwyjnvset.html

const double = x => x * 2;
来源：http://hz.zhixingplan.top/gtnkzcjora.html

[U95] JS：Promise 包装
来源：http://hz.xziqi.cn/gtsvmqyoew.html

new Promise((resolve, reject) => {})
来源：http://hz.aibaodan.cn/gtktmuqpiw.html

[U96] JS：async/await 与异常
来源：http://hz.jinyuanbaomall.cn/gtknnyugyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtphrviisp.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangtech.top/gtuddtuntu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtmrskmlqs.html

[U98] JS：fetch 带 JSON
来源：http://hz.meibo888.top/gtaojmcjgt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.feifeiyinyue.top/gtjoxpnniw.html

[U99] JS：事件监听
来源：http://hz.yj20258888.top/gtlvejolby.html

el.addEventListener("click", e => {})
来源：http://hz.zdqjudy.top/gtslplwsdk.html

[U100] JS：DOM 查询
来源：http://hz.ybcxt.top/gtlhkemhwd.html

document.querySelector(".item")
来源：http://hz.snrcjt.cn/gtcmlijzps.html

[U101] JS：classList 操作
来源：http://hz.redwolf501.top/gtuedavetu.html

el.classList.toggle("active")
来源：http://hz.tanke756.top/gtgiglbwvb.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gtbscwxwgo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jqgfzy.top/gtpmgbuyha.html

[U103] JS：定时器
来源：http://hz.smart0.xyz/gtxsovcmav.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.mhx1999.top/gtdpdacrfj.html

[U104] JS：防抖
来源：http://hz.yj202588.top/gtfdwzaeng.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtuzanqvcu.html

[U105] JS：节流
来源：http://hz.nanxinkj.top/gtplztkhgr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.iojbl.cn/gtlyotiidq.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gtpkhscbrp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yanxiufei.cn/gteeiqvgqx.html

[U107] JS：数字千分位
来源：http://hz.quarkkingdee.top/gtaemwzwxp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.mhx1999.top/gtutwgirjp.html

[U108] JS：随机整数
来源：http://hz.zhixingplan.top/gtdgskxvgk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.c1oappe.top/gtreoxuqdi.html

[U109] JS：数组分组
来源：http://hz.ydzc1.top/gtffgiqnoo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gthogdjrgp.html

[U110] JS：数组分块
来源：http://hz.bjfxy.top/gtkkmdntlg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cdnleiting.top/gtsbjvbhlj.html

[U111] JS：对象转 Map
来源：http://hz.xuetiantiany.cn/gtfqvwolun.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtzrlmfoay.html

[U112] JS：字符串补位
来源：http://hz.fengsongda.top/gtksdsrjzc.html

"7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtvphrwdzd.html

[U113] JS：正则替换全部
来源：http://hz.yuxming.cn/gtpkyymprf.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtjolspqab.html

[U114] JS：JSON 深比较
来源：http://hz.kuanghao11.cn/gttoxecgre.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtufxeyant.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtbixoyuio.html

crypto.randomUUID()
来源：http://hz.xziqi.cn/gtnygohwfx.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhengqikj.top/gtosstwgpd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yongpay.top/gtcnlhmypv.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gttbgyrlof.html

npm i -D vitest;  npx vitest
来源：http://hz.yj20258888.top/gtclajqzwp.html

[U118] JS：开发服务器
来源：http://hz.zhengqikj.top/gtbpwzsmvw.html

npm i -D vite;  npx vite
来源：http://hz.jqgfzy.top/gtclwrywlg.html

[U119] JS：生产构建
来源：http://hz.316326.xyz/gtdjwzpwas.html

npx vite build
来源：http://hz.meibo888.top/gtnlrclkxg.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.guowangkeji.top/gtbkpaqysy.html

import.meta.env.VITE_API_URL
来源：http://hz.52xcode.cn/gtudifqmra.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlvbfllni.html

统计汇总
来源：http://hz.vqdsnc.cn/gtjyidokds.html

================================================================================
来源：http://hz.gotoacloud.top/gtvpqexrvw.html

按语言统计（条）：
来源：http://hz.vqdsnc.cn/gtjrfeirth.html

Python ......... 252
来源：http://hz.wangdashe.top/gtakkyzmqd.html

PHP ............ 252
来源：http://hz.meibo888.top/gtptrgmcyv.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtzxeyrcsn.html

TypeScript ..... 212
来源：http://hz.yj202588.top/gtwbznrksl.html

Java ........... 212
来源：http://hz.nwbrower.top/gtezjsijlt.html

Go ............. 212
来源：http://hz.fengsongda.top/gtcwttmnfz.html

Ruby ........... 212
来源：http://hz.ppjwa.cn/gtyhpvcmmx.html

C# ............. 212
来源：http://hz.cdnleiting.top/gtmtwmemah.html

C .............. 30
来源：http://hz.yongpay.top/gtushzghwd.html

C++ ............ 30
来源：http://hz.chenzaomai.com/gtsykoptex.html

SQL ............ 90
来源：http://hz.birdmap.top/gtzsaqvwyu.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtcejluczi.html

Kotlin ......... 15
来源：http://hz.nwbrower.top/gttkzluefq.html

Swift .......... 15
来源：http://hz.chenzaomai.com/gtqqahqnbb.html

Lua ............ 10
来源：http://hz.gotoacloud.top/gtocqngvkr.html

Perl ........... 10
来源：http://hz.sweek.top/gtmwrvqglh.html

Scala .......... 10
来源：http://hz.wangdashe.top/gttozshyhh.html

------------------------------------
来源：http://hz.jinghuilouyu.cn/gtwejaivea.html

合计 ........... 2106 条
来源：http://hz.pycfn.com/gtowcrxmaz.html

按章节统计：
来源：http://hz.jinqigufen.top/gtzhapjyhr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jiagoushi.top/gtqftnhnmp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtqcjnumle.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hywenlv.cn/gtcntuadxd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtjbpfpduk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhoulong.xyz/gttvmafuwh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.snrcjt.cn/gtfleqpqqq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtwpjspfok.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.316326.xyz/gtfutnbksx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gtvhubhsju.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtbxlhvzeo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtrrekngoi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtlojpeuya.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtbyaciies.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cqqwz.cn/gtvaixfurf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.fzhhl.top/gtdvukousi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtpgkcggfz.html

Q SQL 专题                              90
来源：http://hz.zhixingplan.top/gtrdvitoxa.html

R Bash 专题                             80
来源：http://hz.yonumen.top/gtaxgzdvhd.html

S C / C++ 专题                          60
来源：http://hz.shuidangran.top/gtsfunmugd.html

T 其他语言补充                          60
来源：http://hz.zdqjudy.top/gtfeiwawez.html

U 高频实用片段                         120
来源：http://hz.jinyuanbaomall.cn/gtksaaaujk.html

------------------------------------
来源：http://hz.jinqigufen.top/gtjnzscqxw.html

合计                                  2106 条
来源：http://hz.cashguo.top/gtbscdnfvo.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtzyfklfaj.html

使用提醒
来源：http://hz.xinyue.icu/gtvbianguw.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtmnfxqofv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtagsghboe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.wangdashe.top/gtyvhymktm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhoulong.xyz/gtmeofbiho.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.redwolf501.top/gtedkyjcjd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.smart0.xyz/gtuxsgdzok.html

—— 文件结束 ——
来源：http://hz.daxiang520.top/gtzxssahts.html

================================================================================
来源：http://hz.sysykeji.top/gtfmbmzqmu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jyoumei.cn/gtdytqivam.html

Common Programming Examples Cheat Book
来源：http://hz.zhengqikj.top/gthemqjpor.html

================================================================================
来源：http://hz.ppjwa.cn/gtcuxlldck.html

【收录内容】
来源：http://hz.yonumen.top/gtttpobydp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.gzhubu.top/gtsbenlgfo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.xylfe.cn/gtbunahqns.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gtynblukmy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.daxiang520.top/gtusqwtzzf.html

【使用说明】
来源：http://hz.jlsjyb.cn/gtsyfygwoi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtohvzmuyt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.aibaodan.cn/gtziwhmznh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jqgufenzy.top/gtmyqyyfsh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hnxiangtu.top/gtkvhuzbxu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shzxlz.cn/gtaphzwqgn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hammf.cn/gtcujlphdg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pengpengdd.cyou/gtzeuhlckk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zdqjudy.top/gtyyfsluea.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sweek.top/gtrergkvaw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gtjnmihtbf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.gogol.net.cn/gtpyvlrzrp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nanxinkj.top/gttnggabuv.html

【文件统计】
来源：http://hz.ywan-chungtsiang.top/gtzoqwumjp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jqgfzy.top/gtamrrpjtl.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtlmkvelyj.html

目  录
来源：http://hz.feifeiyinyue.top/gtmswkzcyz.html

--------------------------------------------------------------------------------
来源：http://hz.yuanzhike.top/gtvlqgkqyk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtexihyyry.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gttbctspql.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jianghu66.top/gtrgugddby.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtjdnosdas.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.zdqjudy.top/gtaywrkxjx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.pengpengdd.cyou/gtiyaasokm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hongshengwenyu.top/gtwgokvqnd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xingfuxueyuan.xyz/gtgqrbdlzd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtrvpjhalx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.9152youxi.cn/gtmamyaldr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtbzuisvwn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtzmruzmrp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtggahssqp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yj20258.top/gtyooeudnk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shzxlz.cn/gtbwcaorga.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtoymyynzo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.0kj1m.cn/gtsjdavagt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangtech.top/gtjxixjhin.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.chenlongwang.top/gtwgjejyej.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtpacvhobv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtnrpvudjx.html

================================================================================
来源：http://hz.andypj.xyz/gtdagwzalx.html

A. 基础语法与类型
来源：http://hz.xuetiantiany.cn/gtpwagaqoa.html

================================================================================
来源：http://hz.guowangkeji.top/gttthtvzag.html

[A01] Hello World
来源：http://hz.tanke756.top/gtsteraajz.html

Py:   print("Hello, World!")
来源：http://hz.ydzc1.top/gtlqffdxpp.html

PHP:  echo "Hello, World!";
来源：http://hz.cdnleiting.top/gtbmnjdcle.html

JS:   console.log("Hello, World!");
来源：http://hz.ybcxt.top/gtsszcmbsz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cdnleiting.top/gtuikuiewl.html

Java: System.out.println("Hello, World!");
来源：http://hz.9152youxi.cn/gtebtlbnxy.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhixingplan.top/gtmfbytumg.html

Ruby: puts "Hello, World!"
来源：http://hz.xinyue.icu/gtgwipecik.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.c1oappe.top/gtvxvvekji.html

[A02] 变量声明与赋值
来源：http://hz.shzxlz.cn/gtvrmkxhfl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.chenlongwang.top/gtqkislyer.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuxming.cn/gtynuvoana.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.iojbl.cn/gtqlxccovh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhijiandao.cn/gtnvyjhywx.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydzc1.top/gtwxawgscn.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhengqikj.top/gtupokpbab.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ywan-chungtsiang.top/gtcfllbimm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sysykeji.top/gthszzpsnj.html

[A03] 常量定义
来源：http://hz.fzhhl.top/gtqqwowduq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj20258.top/gtfsagmyxv.html

PHP:  const PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtpdbwqjpk.html

JS:   const PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtlqbxklve.html

TS:   const PI: number = 3.14159;
来源：http://hz.dianchejie.cn/gtfzhgdjmf.html

Java: static final double PI = 3.14159;
来源：http://hz.pycfn.com/gtvpxzesyg.html

Go:   const PI = 3.14159
来源：http://hz.yuanzhike.top/gtcygizokh.html

Ruby: PI = 3.14159
来源：http://hz.jinyuanbaomall.cn/gtovcmnukl.html

C#:   const double PI = 3.14159;
来源：http://hz.jqgfzy.top/gtjjvqyrvr.html

[A04] 判断变量类型
来源：http://hz.cqqwz.cn/gtmhdvbxll.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.havefunace.top/gtaofrevah.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ydjk.org.cn/gtdqtbwlyb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yj20258888.top/gtgfbgahzh.html

TS:   typeof x; x instanceof Date
来源：http://hz.aibaodan.cn/gtzcqdzvdq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.fengsongda.top/gtngklvhsc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yueranfly.top/gtkvdbhenu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tanke756.top/gtkdvgvjtv.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgufenzy.top/gtushrgnxl.html

[A05] 整数除法与取模
来源：http://hz.sweek.top/gtutvjrktn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.pycfn.com/gtwcajzdhe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.tianlin.xyz/gtulfvikid.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gzhubu.top/gtqjmsbczj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtoxtlaftz.html

Java: 7 / 2; 7 % 2
来源：http://hz.feifeiyinyue.top/gtjcywgsbh.html

Go:   7 / 2; 7 % 2
来源：http://hz.sufxvd.cn/gtccmsekpy.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtjpedjqds.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gttmtrecmt.html

[A06] 字符串转数字
来源：http://hz.pycfn.com/gtunlsgfpa.html

Py:   int("42"); float("3.14")
来源：http://hz.cucudq.cn/gtacugecju.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.birdmap.top/gtdakeqqzz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jqgufenzy.top/gtqjmtafxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.tian-w.cn/gtdwflvopt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.gotoacloud.top/gtfwpwitkg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xziqi.cn/gtedoewlzi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.pengpengdd.cyou/gtfssfmmbw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xuetiantiany.cn/gtzodxmbee.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtevsoilaj.html

Py:   str(42)
来源：http://hz.svipenyu.cn/gtqtnxvwys.html

PHP:  (string) 42; strval(42)
来源：http://hz.cucudq.cn/gtpbqhysrp.html

JS:   String(42); (42).toString()
来源：http://hz.yongpay.top/gtyofargmu.html

TS:   String(42)
来源：http://hz.xylfe.cn/gtrjakpmiw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hfpthk.cn/gtbvsdxeik.html

Go:   strconv.Itoa(42)
来源：http://hz.hongshengwenyu.top/gtstbpuxhr.html

Ruby: 42.to_s
来源：http://hz.ppjwa.cn/gtemvynnxs.html

C#:   42.ToString()
来源：http://hz.jyoumei.cn/gtmcadzkjh.html

[A08] 取整与四舍五入
来源：http://hz.chenzaomai.com/gtsyrpibdj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.chenzaomai.com/gtigyqqrfs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.birdmap.top/gtxbawoaps.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtncyqsvwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.sysykeji.top/gtahkyrdrb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xuetiantiany.cn/gthabqttfs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.ehwqpu.com/gtftasiqoj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.fengsongda.top/gtbjksnwns.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hysaishi.cn/gtbqoycqhc.html

[A09] 绝对值与最大最小值
来源：http://hz.yangfankeji.com/gtvcxcnetj.html


<!-- 参考信息 -->