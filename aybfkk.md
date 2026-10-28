代发 wailian999

[U49] PHP：只读属性
来源：http://hz.xuetiantiany.cn/gttmxtbhri.html

public readonly string $name
来源：http://hz.zhijiandao.cn/gtitvpmeuf.html

[U50] PHP：构造器属性提升
来源：http://hz.svipenyu.cn/gtpllbwioe.html

public function __construct(private int $id) {}
来源：http://hz.ydzc1.top/gtudroattb.html

[U51] PHP：数组解构
来源：http://hz.ydjk.org.cn/gtixzmpwiv.html

[$a, $b] = $arr;
来源：http://hz.jiagoushi.top/gtmzbmppdw.html

[U52] PHP：箭头函数
来源：http://hz.smart0.xyz/gtcpcqiwwz.html

$double = fn($x) => $x * 2;
来源：http://hz.gotoacloud.top/gtxindlnon.html

[U53] PHP：空合并运算符
来源：http://hz.chenzaomai.com/gtmtbooyoi.html

$v = $a ?? $b ?? "default";
来源：http://hz.cashguo.top/gtxnqudlsd.html

[U54] PHP：空安全调用
来源：http://hz.xinyue.icu/gtmamibltj.html

$obj?->method()
来源：http://hz.mhx1999.top/gtsiqskrqr.html

[U55] PHP：match 表达式
来源：http://hz.wangshuangyany.cn/gtmunrimvv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.feifeiyinyue.top/gtnwlzjqwp.html

[U56] PHP：命名参数
来源：http://hz.ppjwa.cn/gtnwuiejdz.html

f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtsxusvrca.html

[U57] PHP：字符串插值
来源：http://hz.9152youxi.cn/gtsotulysw.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtbawocypl.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtrgtrdxez.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtteknmmtj.html

[U59] PHP：自定义排序
来源：http://hz.havefunace.top/gtsehcwoqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gttyclohyb.html

[U60] PHP：JSON 编解码
来源：http://hz.jinqigfzy.top/gtbrgzlziy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj202588.top/gthsofbrtk.html

[U61] PHP：正则
来源：http://hz.yonumen.top/gtvycqmnkb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtbvoemvaa.html

[U62] PHP：日期对象
来源：http://hz.mhx1999.top/gtgierfowl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.daria6918.cn/gtzkllbpjs.html

[U63] PHP：文件读写
来源：http://hz.yanxiufei.cn/gtonxtlfif.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenzaomai.com/gtitqwujjy.html

[U64] PHP：目录遍历
来源：http://hz.jinyuanbaomall.cn/gtprupxzlj.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cucudq.cn/gtgwohkcqb.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gttwltwggb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhoulong.xyz/gtgujguwzr.html

[U66] PHP：设置 Cookie
来源：http://hz.zhaomingkeji.xyz/gtxmshxicv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tianlin.xyz/gtdczpbtwb.html

[U67] PHP：处理文件上传
来源：http://hz.xuanzx.com/gtqhaunivu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cashguo.top/gtvfuybtbk.html

[U68] PHP：PDO 连接
来源：http://hz.havefunace.top/gtmzmrafvu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yanxiufei.cn/gtszoymhch.html

[U69] PHP：PDO 预处理
来源：http://hz.haohaochexian.top/gtrauzmkjs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ywan-chungtsiang.top/gtwjshibhc.html

[U70] PHP：PDO 事务
来源：http://hz.c1oappe.top/gtapedtenc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.mhx1999.top/gtvcavdmmc.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangkeji.top/gtyehmoiwi.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenzaomai.com/gtldxsjpqf.html

[U72] PHP：写错误日志
来源：http://hz.pycfn.com/gtkzcneryv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.quarkkingdee.top/gtqvzyrhxv.html

[U73] PHP：读取 ini 配置
来源：http://hz.ybcxt.top/gtdoujxnnb.html

parse_ini_file("config.ini", true)
来源：http://hz.ydjk.org.cn/gtspctpiqp.html

[U74] PHP：读取环境变量
来源：http://hz.guowangkeji.top/gtssrfgqop.html

getenv("APP_ENV") ?: "production"
来源：http://hz.dianchejie.cn/gtuvrlixxd.html

[U75] PHP：依赖注入
来源：http://hz.kuanghao11.cn/gtrfoefklf.html

composer require psr/container
来源：http://hz.yuanzhike.top/gtrydcnptu.html

[U76] PHP：简单路由
来源：http://hz.mhx1999.top/gtpadmcpfh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.yueranfly.top/gtbxwokjep.html

[U77] PHP：模板渲染
来源：http://hz.wangshuangyany.cn/gtoltbyfmm.html

composer require twig/twig
来源：http://hz.hammf.cn/gtvpteaors.html

[U78] PHP：单元测试
来源：http://hz.daria6918.cn/gtrsmwhqqq.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtekziborc.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtaygscauy.html

composer require --dev phpstan/phpstan
来源：http://hz.chenlongwang.top/gtyfreukdm.html

[U80] PHP：代码规范修复
来源：http://hz.yangfankeji.com/gtczhtkjyg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xylfe.cn/gtlrcnzrsa.html

[U81] JS：初始化项目
来源：http://hz.jyoumei.cn/gtaqukusys.html

npm init -y;  npm i express
来源：http://hz.wangdashe.top/gtdulurfjm.html

[U82] JS：package.json 脚本
来源：http://hz.fzhhl.top/gtttelkqqn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.aibaodan.cn/gtcfykzcay.html

[U83] JS：ES Module 导入导出
来源：http://hz.jqgufenzy.top/gttgucwujj.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shzxlz.cn/gtszuheves.html

[U84] JS：CommonJS 写法
来源：http://hz.guannengcc.top/gtwrxzydis.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.jinqigfzy.top/gthxfvprxm.html

[U85] JS：可选链
来源：http://hz.sysykeji.top/gttakwdaia.html

a?.b?.c
来源：http://hz.nanxuanxn.top/gtfyzojlya.html

[U86] JS：空值合并
来源：http://hz.yj20258888.top/gtglvdrouk.html

a ?? b
来源：http://hz.zhixingplan.top/gtuoksblry.html

[U87] JS：解构默认值
来源：http://hz.andypj.xyz/gtnllfrwdm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tianlin.xyz/gtdkzcqdob.html

[U88] JS：对象展开合并
来源：http://hz.hnxiangtu.top/gtupnbavgw.html

{ ...a, ...b }
来源：http://hz.cashguo.top/gtukcmztca.html

[U89] JS：数组去重
来源：http://hz.xziqi.cn/gtvygpjpjq.html

[...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtttrphxhg.html

[U90] JS：数字数组排序
来源：http://hz.haohaochexian.top/gtobbhvlbq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtrzirovzx.html

[U91] JS：对象键值遍历
来源：http://hz.52xcode.cn/gtckgyqspd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenjidiqi.icu/gtqonoqfks.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gtldflafmc.html

structuredClone(obj)
来源：http://hz.sweek.top/gtykummgru.html

[U93] JS：模板字符串
来源：http://hz.quarkkingdee.top/gtsegnkcef.html

`共 ${n} 条`
来源：http://hz.wangdashe.top/gtgcqazcvr.html

[U94] JS：箭头函数
来源：http://hz.zdqjudy.top/gtsmtwkumu.html

const double = x => x * 2;
来源：http://hz.0kj1m.cn/gtspmxqplx.html

[U95] JS：Promise 包装
来源：http://hz.haohaochexian.top/gtdzygbekz.html

new Promise((resolve, reject) => {})
来源：http://hz.zhongyouzk.top/gtisxbouys.html

[U96] JS：async/await 与异常
来源：http://hz.hysaishi.cn/gtdivwumrp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtamhzuchr.html

[U97] JS：并发请求
来源：http://hz.xingfuxueyuan.xyz/gtqtbgqlat.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtwtjtvmqq.html

[U98] JS：fetch 带 JSON
来源：http://hz.sweek.top/gtnijatgst.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daria6918.cn/gtqqdjaert.html

[U99] JS：事件监听
来源：http://hz.fengsongda.top/gtqwpsdsbe.html

el.addEventListener("click", e => {})
来源：http://hz.ybcxt.top/gtfrsoifyf.html

[U100] JS：DOM 查询
来源：http://hz.wangdashe.top/gtqzthwnei.html

document.querySelector(".item")
来源：http://hz.cashguo.top/gtshqqeice.html

[U101] JS：classList 操作
来源：http://hz.shangyingyoupin.top/gtocedzupm.html

el.classList.toggle("active")
来源：http://hz.jinqigufen.top/gtsqbmotbp.html

[U102] JS：本地存储
来源：http://hz.xingfuxueyuan.xyz/gtvnstucto.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtowjgrzuo.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtteffmrzj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cucudq.cn/gtgbaeaghw.html

[U104] JS：防抖
来源：http://hz.yueranfly.top/gtmcmiqhpr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtdmewogie.html

[U105] JS：节流
来源：http://hz.ehwqpu.com/gtkvceluod.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hywenlv.cn/gtaldsjeae.html

[U106] JS：日期格式化
来源：http://hz.xinyue.icu/gtfgzguweg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.meibo888.top/gtecjxoopw.html

[U107] JS：数字千分位
来源：http://hz.ywan-chungtsiang.top/gttddigbzz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ydjk.org.cn/gtathkpidi.html

[U108] JS：随机整数
来源：http://hz.jlsjyb.cn/gtwlijxsuy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hammf.cn/gtjsqluuho.html

[U109] JS：数组分组
来源：http://hz.ppjwa.cn/gtdhebsbck.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtdnhpfvjj.html

[U110] JS：数组分块
来源：http://hz.cdnleiting.top/gtnclgezcl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shzxlz.cn/gtvcpomuze.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtkblkbkql.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtwddbrkht.html

[U112] JS：字符串补位
来源：http://hz.xinyue.icu/gtycuwfvzj.html

"7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtokowgyez.html

[U113] JS：正则替换全部
来源：http://hz.0kj1m.cn/gtnxnnfdyc.html

s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtwadnyzvy.html

[U114] JS：JSON 深比较
来源：http://hz.birdmap.top/gtcmouaorr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.guannengcc.top/gtwneomtfx.html

[U115] JS：生成 UUID
来源：http://hz.c1oappe.top/gtqpuajdbl.html

crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtpwfqguqo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.aibaodan.cn/gthtcqbrgs.html

/** @param {string} name */ function f(name) {}
来源：http://hz.fengsongda.top/gtxaovadij.html

[U117] JS：单元测试
来源：http://hz.xuetiantiany.cn/gtrntqlxpc.html

npm i -D vitest;  npx vitest
来源：http://hz.zhixingplan.top/gtnxjbjplu.html

[U118] JS：开发服务器
来源：http://hz.aibaodan.cn/gtfvjpgumk.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gtmlmwfeib.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gtoqiafbtr.html

npx vite build
来源：http://hz.zhaomingkeji.xyz/gtyqzlzfax.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.wangdashe.top/gtlimzwogh.html

import.meta.env.VITE_API_URL
来源：http://hz.daria6918.cn/gtmdinwjxq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxlpacbjb.html

统计汇总
来源：http://hz.52xcode.cn/gtcttzfsdl.html

================================================================================
来源：http://hz.9152youxi.cn/gtdytgiuij.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtrbdovtsm.html

Python ......... 252
来源：http://hz.hysaishi.cn/gtamxfmbru.html

PHP ............ 252
来源：http://hz.aibaodan.cn/gtazuncspk.html

JavaScript ..... 252
来源：http://hz.yanxiufei.cn/gtwtsdmplz.html

TypeScript ..... 212
来源：http://hz.wangshuangyany.cn/gtjvitrlbx.html

Java ........... 212
来源：http://hz.cdnleiting.top/gtdejwlrhj.html

Go ............. 212
来源：http://hz.tian-w.cn/gtvginlvuj.html

Ruby ........... 212
来源：http://hz.yangfankeji.com/gtxmirqvjm.html

C# ............. 212
来源：http://hz.kuanghao11.cn/gtvtiklgox.html

C .............. 30
来源：http://hz.nanxinkj.top/gtcmezoqzs.html

C++ ............ 30
来源：http://hz.zhengqikj.top/gthdjrfmln.html

SQL ............ 90
来源：http://hz.andypj.xyz/gtspvvffzc.html

Bash ........... 80
来源：http://hz.hnqzz.top/gtshpdcgzv.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtykrztvkm.html

Swift .......... 15
来源：http://hz.cqqwz.cn/gtgkptksss.html

Lua ............ 10
来源：http://hz.pycfn.com/gtrwejrzcl.html

Perl ........... 10
来源：http://hz.pengpengdd.cyou/gtwweilyjz.html

Scala .......... 10
来源：http://hz.redwolf501.top/gtpzbjenri.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtfeilmiqg.html

合计 ........... 2106 条
来源：http://hz.jqgufenzy.top/gtkwyitlcf.html

按章节统计：
来源：http://hz.gzhubu.top/gttbdgygvt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nanxinkj.top/gtgcgpzivm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtyxywrezv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtuswlhkki.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtodffzeqp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhixingplan.top/gtnvimtfpb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.birdmap.top/gtmqqhsqrv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtfsgiqbai.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gteaohemsk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtbkeeeyvi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtxsdfatom.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtucrpaxrw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtrcwslraa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtaueoucvs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtbiewgvhc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtlirbpzbg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtoacrablu.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gthlfzfwse.html

R Bash 专题                             80
来源：http://hz.ydzc1.top/gtbzhqcdpv.html

S C / C++ 专题                          60
来源：http://hz.yj20258888.top/gtsquililt.html

T 其他语言补充                          60
来源：http://hz.yongpay.top/gtjvabmnac.html

U 高频实用片段                         120
来源：http://hz.nanxinkj.top/gtydgjjvnf.html

------------------------------------
来源：http://hz.yvedp.cn/gtcrtatsac.html

合计                                  2106 条
来源：http://hz.jqgufenzy.top/gtxrdiucbd.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtghpdpoya.html

使用提醒
来源：http://hz.shuidangran.top/gtkniezlyy.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gttyurwhxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yuxming.cn/gtxpudqrhw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenjidiqi.icu/gtaakeedba.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.snrcjt.cn/gtyauwaess.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hnqzz.top/gtmdplwozc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jiagoushi.top/gtmrqfvaug.html

—— 文件结束 ——
来源：http://hz.jyoumei.cn/gtrptfjnha.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmnwvwwcx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tanke756.top/gtffbvreul.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gtbjewkmdw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmptclxek.html

【收录内容】
来源：http://hz.daxiang520.top/gttnivkmqt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.kuanghao11.cn/gtiunttvyy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhijiandao.cn/gtowcbjmzs.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gtvkrvkwlv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cheryme.top/gtxhabjcbc.html

【使用说明】
来源：http://hz.jlsjyb.cn/gtathlzirq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.vqdsnc.cn/gtusyfohpq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cdnleiting.top/gtojonhnwt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yueranfly.top/gtcvmlazet.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jlsjyb.cn/gthbjxplpu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.kuanghao11.cn/gtdygoasaj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuxming.cn/gtnpdmqvmz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangkeji.top/gtomugfgbe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.dianchejie.cn/gtcdthnplg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuanzhike.top/gtaileiwtg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yangfankeji.com/gtmjxndpkt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhongyouzk.top/gtvhzsxfte.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yuxming.cn/gtsbvwcxeh.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtlwtxsugj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cashguo.top/gtbpniuood.html

--------------------------------------------------------------------------------
来源：http://hz.c1oappe.top/gtuvoezdms.html

目  录
来源：http://hz.zhixingplan.top/gtpmfuckhb.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtwqquyovo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gthxkfliir.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtgwbsgres.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtbzmsoqgt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.0kj1m.cn/gtacoijxma.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shangyingyoupin.top/gtymkzxvfj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ehwqpu.com/gtwgzvowdo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinqigufen.top/gtzmhhllvq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xylfe.cn/gtrkqwqrnj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtyxonofuw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtwjxmjjhl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtqchcwdwh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtzlhwuiaf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtuapgpgwl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.gaohongyu789.top/gtbmhckyeg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.dianchejie.cn/gtwvwurggn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gtbaqtebcd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.wangshuangyany.cn/gttlkfyylt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhixingplan.top/gtoaovktca.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xinyue.icu/gtmjvvxnbk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtisffzlfz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jyoumei.cn/gteglmjjoq.html

================================================================================
来源：http://hz.gotoacloud.top/gtldngjgbi.html

A. 基础语法与类型
来源：http://hz.yj20258.top/gtrtfjrwqo.html

================================================================================
来源：http://hz.cdnleiting.top/gtjwmvulea.html

[A01] Hello World
来源：http://hz.cdnleiting.top/gtmcmuwswy.html

Py:   print("Hello, World!")
来源：http://hz.sysykeji.top/gtnwsylnmv.html

PHP:  echo "Hello, World!";
来源：http://hz.yuanzhike.top/gthexaapcm.html

JS:   console.log("Hello, World!");
来源：http://hz.meibo888.top/gtykwzmyha.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.svipenyu.cn/gtyosciyky.html

Java: System.out.println("Hello, World!");
来源：http://hz.redwolf501.top/gtfonjbvbh.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cqqwz.cn/gtpdsrpakl.html

Ruby: puts "Hello, World!"
来源：http://hz.sweek.top/gtnpqmxzle.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.quarkkingdee.top/gtvlmjfrmq.html

[A02] 变量声明与赋值
来源：http://hz.ppjwa.cn/gtbzgwvbnc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jinqigufen.top/gtxrtwgwth.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fzhhl.top/gtuvzerpmv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.guannengcc.top/gtyoyzzfst.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.guowangkeji.top/gttjuwtdyv.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hnxiangtu.top/gtmejdvssi.html

Go:   name := "Alex"; age := 20
来源：http://hz.gzhubu.top/gtrnrcbbem.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jlsjyb.cn/gtsxyragkg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtngqbkhrj.html

[A03] 常量定义
来源：http://hz.zdqjudy.top/gttcbzkigk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yj202588.top/gtvhrbnski.html

PHP:  const PI = 3.14159;
来源：http://hz.havefunace.top/gtidrtebsk.html

JS:   const PI = 3.14159;
来源：http://hz.bjfxy.top/gtjgcldcqh.html

TS:   const PI: number = 3.14159;
来源：http://hz.yangfankeji.com/gtmonnivbj.html

Java: static final double PI = 3.14159;
来源：http://hz.tian-w.cn/gttwmxcnsw.html

Go:   const PI = 3.14159
来源：http://hz.nwbrower.top/gtmuxemycr.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtoiqucyot.html

C#:   const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtbphyumjl.html

[A04] 判断变量类型
来源：http://hz.cheryme.top/gtahenrmjo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jyoumei.cn/gtsncnosci.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.sysykeji.top/gtpyeckfgh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yueranfly.top/gtjqndjvop.html

TS:   typeof x; x instanceof Date
来源：http://hz.nwbrower.top/gtsvuahpor.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.andypj.xyz/gtvvgxhwuz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.guannengcc.top/gtvfvrlckb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xylfe.cn/gttsunscjj.html

C#:   x.GetType().Name; x is int
来源：http://hz.yuanzhike.top/gtuagokoap.html

[A05] 整数除法与取模
来源：http://hz.sufxvd.cn/gtvkymlxgw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.c1oappe.top/gtjcvoxftx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.vqdsnc.cn/gtrtcegvta.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.andypj.xyz/gtpokswgeb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.pycfn.com/gtbfjwwyef.html

Java: 7 / 2; 7 % 2
来源：http://hz.52xcode.cn/gtcxzwxzle.html

Go:   7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gtuzcjaywm.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yj202588.top/gthewhsitg.html

C#:   7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtxiorbbbx.html

[A06] 字符串转数字
来源：http://hz.yangfankeji.com/gtqaxjdiiv.html

Py:   int("42"); float("3.14")
来源：http://hz.jyoumei.cn/gtyzacjnty.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cdnleiting.top/gtuvpnvkcy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.316326.xyz/gtrjeqoasv.html


<!-- 参考信息 -->