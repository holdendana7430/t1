代发 wailian999

[U31] Py：单测
来源：http://hz.jinyuanbaomall.cn/gtgwkbdzuq.html

python -m pytest -q
来源：http://hz.zhengqikj.top/gtjwzpneqb.html

[U32] Py：代码格式化
来源：http://hz.jinghuilouyu.cn/gtbnozrrhq.html

ruff format . && ruff check --fix .
来源：http://hz.cucudq.cn/gtgoypwcbt.html

[U33] Py：打包发布
来源：http://hz.zhiwuduotai.top/gtyogxubbj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhijiandao.cn/gtiavadcty.html

[U34] Py：判断编码
来源：http://hz.zycfv.cn/gtouhauyyp.html

chardet.detect(raw)
来源：http://hz.fzhhl.top/gtgwwwevxq.html

[U35] Py：发送邮件
来源：http://hz.chenzaomai.com/gtejyrvnuq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtpmizulum.html

[U36] Py：定时任务
来源：http://hz.redwolf501.top/gtufcvjgfo.html

schedule.every(10).minutes.do(job)
来源：http://hz.sweek.top/gtousrcszm.html

[U37] Py：读写 Excel
来源：http://hz.birdmap.top/gtfynnxkfn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.andypj.xyz/gtvzhdpdln.html

[U38] Py：获取脚本所在目录
来源：http://hz.shangyingyoupin.top/gtltubhfut.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtubiinomo.html

[U39] Py：判断是否在交互环境
来源：http://hz.shzxlz.cn/gtfgpxrteg.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtmeveuzin.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtxctcdtcp.html

print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtmrarkflu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ywan-chungtsiang.top/gtwdsiioup.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtfrxudjlk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtlwtexvrx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gtcksmyojx.html

[U43] PHP：声明命名空间
来源：http://hz.aibaodan.cn/gthkrnnhyu.html

namespace App\Http;
来源：http://hz.bjfxy.top/gtiwmuawue.html

[U44] PHP：开启严格类型
来源：http://hz.haohaochexian.top/gtnfyaetrj.html

declare(strict_types=1);
来源：http://hz.andypj.xyz/gtzoltmqcc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cheryme.top/gtjyktlsvn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtlzcdojde.html

[U46] PHP：可空类型
来源：http://hz.svipenyu.cn/gtjkacezvk.html

?string $name = null
来源：http://hz.dashuyun.cn/gtvtwenozm.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangtech.top/gtvbhbltkf.html

int|string $id
来源：http://hz.feifeiyinyue.top/gtobqnjcig.html

[U48] PHP：纯枚举
来源：http://hz.zhiwuduotai.top/gturpoxwqk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.iojbl.cn/gtoxfqvkol.html

[U49] PHP：只读属性
来源：http://hz.jianghu66.top/gtizleumkm.html

public readonly string $name
来源：http://hz.fzhhl.top/gttfowckek.html

[U50] PHP：构造器属性提升
来源：http://hz.gogol.net.cn/gtyzqimixg.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtddidhzci.html

[U51] PHP：数组解构
来源：http://hz.zhiwuduotai.top/gtzsohfbpt.html

[$a, $b] = $arr;
来源：http://hz.hnxiangtu.top/gtaktorrja.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtukhflwqb.html

$double = fn($x) => $x * 2;
来源：http://hz.yonumen.top/gtrfrsklpf.html

[U53] PHP：空合并运算符
来源：http://hz.zhixingplan.top/gtxhoxoftp.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuxming.cn/gtjrqkvwju.html

[U54] PHP：空安全调用
来源：http://hz.andypj.xyz/gtkyeyxghe.html

$obj?->method()
来源：http://hz.iojbl.cn/gtfbvwtwmo.html

[U55] PHP：match 表达式
来源：http://hz.havefunace.top/gtyzjatzeg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cheryme.top/gtaavjevsa.html

[U56] PHP：命名参数
来源：http://hz.haohaochexian.top/gtarypfigw.html

f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtfgvuqijp.html

[U57] PHP：字符串插值
来源：http://hz.chenlongwang.top/gtkmtdgtyy.html

"值: {$a}"
来源：http://hz.cucudq.cn/gtdphuigjm.html

[U58] PHP：数组三件套
来源：http://hz.zhiwuduotai.top/gtnchfpvik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.9152youxi.cn/gtvqfeqeuj.html

[U59] PHP：自定义排序
来源：http://hz.cdnleiting.top/gtekkuaddx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtorjxeiqq.html

[U60] PHP：JSON 编解码
来源：http://hz.birdmap.top/gtcevcomre.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hfpthk.cn/gtdmwbucmp.html

[U61] PHP：正则
来源：http://hz.jinqigfzy.top/gtdstbiksp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtgwfrjqpf.html

[U62] PHP：日期对象
来源：http://hz.hnqzz.top/gtdhldvmop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zycfv.cn/gtcaahiwcp.html

[U63] PHP：文件读写
来源：http://hz.hnxiangtu.top/gtwgudbcbs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.svipenyu.cn/gtydoebqqv.html

[U64] PHP：目录遍历
来源：http://hz.c1oappe.top/gtblihrvec.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.fengsongda.top/gtkrnwjfdo.html

[U65] PHP：会话
来源：http://hz.9152youxi.cn/gtytjlvvhw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gtwaezioeb.html

[U66] PHP：设置 Cookie
来源：http://hz.hnxiangtu.top/gtqalayglm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.sxryk.cn/gttfxfdqwb.html

[U67] PHP：处理文件上传
来源：http://hz.ydzc1.top/gtliqnxzow.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yuanzhike.top/gtxqeaxbuo.html

[U68] PHP：PDO 连接
来源：http://hz.hywenlv.cn/gtbrjivyhg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jlsjyb.cn/gtiikbtdmg.html

[U69] PHP：PDO 预处理
来源：http://hz.zhoulong.xyz/gtuiimicst.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jinyuanbaomall.cn/gtxentnxvm.html

[U70] PHP：PDO 事务
来源：http://hz.mhx1999.top/gtmlmigvgb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hywenlv.cn/gtlbubbdvl.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtodswvjqc.html

throw new RuntimeException("失败", 500);
来源：http://hz.shanyushiyangtech.top/gtzpxdccqz.html

[U72] PHP：写错误日志
来源：http://hz.yangfankeji.com/gtiuarrhnj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yanxiufei.cn/gtqnpbpfqh.html

[U73] PHP：读取 ini 配置
来源：http://hz.andypj.xyz/gtmnqyyrmu.html

parse_ini_file("config.ini", true)
来源：http://hz.yueranfly.top/gtrzwmulqe.html

[U74] PHP：读取环境变量
来源：http://hz.smart0.xyz/gtmyfiffid.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gtjalmiwou.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtxwfdwpsd.html

composer require psr/container
来源：http://hz.haohaochexian.top/gtcmtxqful.html

[U76] PHP：简单路由
来源：http://hz.zhixingplan.top/gtdopakomy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jianghu66.top/gtpbvnlcdj.html

[U77] PHP：模板渲染
来源：http://hz.yanxiufei.cn/gturdaibkv.html

composer require twig/twig
来源：http://hz.hnqzz.top/gtgvusycta.html

[U78] PHP：单元测试
来源：http://hz.daria6918.cn/gtovxabyhs.html

composer require --dev phpunit/phpunit
来源：http://hz.fzhhl.top/gtzyzscsdq.html

[U79] PHP：静态分析
来源：http://hz.52xcode.cn/gtkamsnpfk.html

composer require --dev phpstan/phpstan
来源：http://hz.hammf.cn/gtwiwpdikn.html

[U80] PHP：代码规范修复
来源：http://hz.shanyushiyangkeji.top/gthzofgjhh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.316326.xyz/gtwfdkbsvh.html

[U81] JS：初始化项目
来源：http://hz.hammf.cn/gtvidrhpkg.html

npm init -y;  npm i express
来源：http://hz.yangfankeji.com/gtwiqiwrld.html

[U82] JS：package.json 脚本
来源：http://hz.tianlin.xyz/gtlxdufirc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.fzhhl.top/gtsvfvteyn.html

[U83] JS：ES Module 导入导出
来源：http://hz.haohaochexian.top/gtigwkdite.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.smart0.xyz/gtbreaosam.html

[U84] JS：CommonJS 写法
来源：http://hz.chenlongwang.top/gthwaclfvn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.tianlin.xyz/gtexclzpnm.html

[U85] JS：可选链
来源：http://hz.zhongyouzk.top/gtboceqeiz.html

a?.b?.c
来源：http://hz.fengsongda.top/gtvbcjrtoi.html

[U86] JS：空值合并
来源：http://hz.zhongyouzk.top/gtkbqnmizk.html

a ?? b
来源：http://hz.yuxming.cn/gtsmhacafw.html

[U87] JS：解构默认值
来源：http://hz.xinyue.icu/gtxizaaqnh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.wangshuangyany.cn/gttzgvhxkn.html

[U88] JS：对象展开合并
来源：http://hz.xingfuxueyuan.xyz/gtypmuchvj.html

{ ...a, ...b }
来源：http://hz.hongshengwenyu.top/gtjrthhvzm.html

[U89] JS：数组去重
来源：http://hz.andypj.xyz/gtwsjjxfwd.html

[...new Set(arr)]
来源：http://hz.jyoumei.cn/gtvebaasjc.html

[U90] JS：数字数组排序
来源：http://hz.cheryme.top/gtkerifbcu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtpllvozeh.html

[U91] JS：对象键值遍历
来源：http://hz.jinghuilouyu.cn/gtzfafznwt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.quarkkingdee.top/gtridhjisn.html

[U92] JS：深拷贝
来源：http://hz.ivvv.top/gtqpipltzc.html

structuredClone(obj)
来源：http://hz.ehwqpu.com/gtzfvnccmk.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtdzofxkkw.html

`共 ${n} 条`
来源：http://hz.tanke756.top/gtmhvvmtqt.html

[U94] JS：箭头函数
来源：http://hz.zhengqikj.top/gtdqjmkedh.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gtkyxqapsu.html

[U95] JS：Promise 包装
来源：http://hz.yuanzhike.top/gtovdaroka.html

new Promise((resolve, reject) => {})
来源：http://hz.yuanzhike.top/gtlloddusy.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtliluujcg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtbxvoobcj.html

[U97] JS：并发请求
来源：http://hz.hammf.cn/gtkmooxxbd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtbbeljlwu.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtjzgpnflg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.chenjidiqi.icu/gtojguveln.html

[U99] JS：事件监听
来源：http://hz.zhijiandao.cn/gtznnfkugm.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258888.top/gtgmnbiysh.html

[U100] JS：DOM 查询
来源：http://hz.ywan-chungtsiang.top/gttsvvmgku.html

document.querySelector(".item")
来源：http://hz.zhoulong.xyz/gtnqrgkvum.html

[U101] JS：classList 操作
来源：http://hz.xuanzx.com/gtugijxmso.html

el.classList.toggle("active")
来源：http://hz.xziqi.cn/gttjwvscln.html

[U102] JS：本地存储
来源：http://hz.ywan-chungtsiang.top/gtapstxsmi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj20258888.top/gtszdqhrkc.html

[U103] JS：定时器
来源：http://hz.tianlin.xyz/gtdfsvkvwu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dianchejie.cn/gtoayjgpat.html

[U104] JS：防抖
来源：http://hz.andypj.xyz/gtbkagcwkz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtzuayycfs.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtbxmpmatf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigfzy.top/gtkljjnvwb.html

[U106] JS：日期格式化
来源：http://hz.xuetiantiany.cn/gtyhmwevsc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gtofaabass.html

[U107] JS：数字千分位
来源：http://hz.hnqzz.top/gtvbusbihu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tian-w.cn/gttjshmvgi.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtrjqugxns.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jyoumei.cn/gtikkqjgmf.html

[U109] JS：数组分组
来源：http://hz.shuidangran.top/gtngygcovn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ydjk.org.cn/gtkrjfqziv.html

[U110] JS：数组分块
来源：http://hz.guowangkeji.top/gtofrwxsdw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.pengpengdd.cyou/gtgasjfmvy.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gtrbycznkq.html

new Map(Object.entries(obj))
来源：http://hz.guowangkeji.top/gtvjgxvqkb.html

[U112] JS：字符串补位
来源：http://hz.jinqigufen.top/gtejxlqfkt.html

"7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtazuwkmgc.html

[U113] JS：正则替换全部
来源：http://hz.zhengqikj.top/gtfhhdmatm.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtyducnlha.html

[U114] JS：JSON 深比较
来源：http://hz.zhijiandao.cn/gttuokgnuq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.tianlin.xyz/gtzycyjdvh.html

[U115] JS：生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtmqurczrm.html

crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtnljrzvxu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hysaishi.cn/gtwwvogmxn.html

/** @param {string} name */ function f(name) {}
来源：http://hz.hnqzz.top/gtwltkgypa.html

[U117] JS：单元测试
来源：http://hz.0kj1m.cn/gtbpwzxqai.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtktbmtjyp.html

[U118] JS：开发服务器
来源：http://hz.jlsjyb.cn/gtadnbften.html

npm i -D vite;  npx vite
来源：http://hz.hywenlv.cn/gtuconzklh.html

[U119] JS：生产构建
来源：http://hz.andypj.xyz/gtarmrwvhu.html

npx vite build
来源：http://hz.zhiwuduotai.top/gtrzcikjiz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gtnevxtiqy.html

import.meta.env.VITE_API_URL
来源：http://hz.xinyue.icu/gtuknouufs.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgtgdwlnm.html

统计汇总
来源：http://hz.hfpthk.cn/gtmuaimxbj.html

================================================================================
来源：http://hz.yj20258.top/gtxpxhlmvw.html

按语言统计（条）：
来源：http://hz.wangdashe.top/gtvvtqlhuv.html

Python ......... 252
来源：http://hz.shzxlz.cn/gtgsnxildu.html

PHP ............ 252
来源：http://hz.fzhhl.top/gtxyyyuoid.html

JavaScript ..... 252
来源：http://hz.nanxuanxn.top/gtxvapaiwr.html

TypeScript ..... 212
来源：http://hz.jinqigfzy.top/gtufrzfurm.html

Java ........... 212
来源：http://hz.smart0.xyz/gtkzwcpzyq.html

Go ............. 212
来源：http://hz.hfpthk.cn/gttwjflies.html

Ruby ........... 212
来源：http://hz.jianghu66.top/gtfcwxivau.html

C# ............. 212
来源：http://hz.sweek.top/gtctydcikx.html

C .............. 30
来源：http://hz.wangdashe.top/gtvvpququw.html

C++ ............ 30
来源：http://hz.hammf.cn/gtmuccggaf.html

SQL ............ 90
来源：http://hz.cdnleiting.top/gttjmrohzv.html

Bash ........... 80
来源：http://hz.chenzaomai.com/gtsggefzft.html

Kotlin ......... 15
来源：http://hz.ydzc1.top/gtfcflrifd.html

Swift .......... 15
来源：http://hz.jiagoushi.top/gtltdbmikk.html

Lua ............ 10
来源：http://hz.shanyushiyangkeji.top/gtxaizaetc.html

Perl ........... 10
来源：http://hz.c1oappe.top/gtvfdghwzu.html

Scala .......... 10
来源：http://hz.snrcjt.cn/gtxgtqmxvv.html

------------------------------------
来源：http://hz.hnqzz.top/gtksdjzasy.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gthrxztiuo.html

按章节统计：
来源：http://hz.daxiang520.top/gtzuvwqyan.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.aibaodan.cn/gtxehqxrwb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtaqgvapet.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtvejhupvx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.meibo888.top/gtjebxzwqt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.quarkkingdee.top/gtbivuknxo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtajixjjhq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtpocuzjen.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtjhlejzws.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.mhx1999.top/gtclhpyvbl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hfpthk.cn/gtywkzzqqp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtqptcxegj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtislflriq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jqgufenzy.top/gtrhqcghnz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtnbukecnj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.dianchejie.cn/gtppzeflra.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtxgomawid.html

Q SQL 专题                              90
来源：http://hz.cdnleiting.top/gtvdtxweln.html

R Bash 专题                             80
来源：http://hz.kuanghao11.cn/gtcfhizxds.html

S C / C++ 专题                          60
来源：http://hz.chenjidiqi.icu/gtlnkvngfx.html

T 其他语言补充                          60
来源：http://hz.zhijiandao.cn/gtmmrosvbz.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gttyskhqat.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtczunlvfq.html

合计                                  2106 条
来源：http://hz.cqqwz.cn/gtmkwtiihy.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gttofzbmkf.html

使用提醒
来源：http://hz.fzhhl.top/gtsfpvehpd.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtdpcwrddb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yangfankeji.com/gtpywlvdkp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xingfuxueyuan.xyz/gtonxknfrw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cqqwz.cn/gtipswmeln.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jqgfzy.top/gthpqcidai.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhongyouzk.top/gtfzqzjoih.html

—— 文件结束 ——
来源：http://hz.ehwqpu.com/gtdtukqqgk.html

================================================================================
来源：http://hz.daria6918.cn/gtzvjwtwek.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.yvedp.cn/gtxdaspoqs.html

Common Programming Examples Cheat Book
来源：http://hz.xinyue.icu/gttuozfzvw.html

================================================================================
来源：http://hz.cheryme.top/gthpwirxkj.html

【收录内容】
来源：http://hz.cashguo.top/gtnuuqioee.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ivvv.top/gttvfmdhkq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cashguo.top/gtsxiljrau.html

SQL · Bash · C · C++
来源：http://hz.zhaomingkeji.xyz/gtbckboety.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.haohaochexian.top/gtccnayfga.html

【使用说明】
来源：http://hz.dianchejie.cn/gtekftjqde.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.snrcjt.cn/gtaypmkvel.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhixingplan.top/gtqtazrvrx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hammf.cn/gtyvrvugjh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.52xcode.cn/gtofpgjrfe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.smart0.xyz/gttgcjacwm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinyuanbaomall.cn/gtzzhcokia.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hnqzz.top/gthwkbzhws.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj20258.top/gthgtekgno.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhoulong.xyz/gtyyphrqjl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gzhubu.top/gtywcxewox.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xziqi.cn/gtcrrgpitx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aibaodan.cn/gtmrytkmuw.html

【文件统计】
来源：http://hz.xziqi.cn/gtrapbvaen.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ehwqpu.com/gtsdpxpxxd.html

--------------------------------------------------------------------------------
来源：http://hz.tanke756.top/gtnwpodsss.html

目  录
来源：http://hz.cdnleiting.top/gtteoxboah.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtlwjadjoe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ppjwa.cn/gttrwatgjs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtoufjhzeg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtfvqkdpiy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cucudq.cn/gtjhdnbhgs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.smart0.xyz/gtreutlbnc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jinqigfzy.top/gtqcbcfvqn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtwyzyzgrg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.daxiang520.top/gtivxnglzz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtivyaevkb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.mhx1999.top/gtzhxcqoux.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtadljaymy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtcxatucxs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtmkfipmjn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gtviqcaaaq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.nwbrower.top/gtdtjwrufn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtuxcthjtr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuetiantiany.cn/gtbfjdnlnv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cheryme.top/gtyhppdqsv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxinkj.top/gtmjvrmhjl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtynpjjcvq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.andypj.xyz/gtkaaotocb.html

================================================================================
来源：http://hz.daxiang520.top/gtukccllbp.html

A. 基础语法与类型
来源：http://hz.yuanzhike.top/gtovelpwmv.html

================================================================================
来源：http://hz.xuanzx.com/gtdmfzcejr.html

[A01] Hello World
来源：http://hz.dianchejie.cn/gtvrmzozke.html

Py:   print("Hello, World!")
来源：http://hz.c1oappe.top/gtexqglbkz.html

PHP:  echo "Hello, World!";
来源：http://hz.zycfv.cn/gtpnmcvrhe.html

JS:   console.log("Hello, World!");
来源：http://hz.yonumen.top/gtlaftxhhd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.9152youxi.cn/gtxrseaurk.html

Java: System.out.println("Hello, World!");
来源：http://hz.pengpengdd.cyou/gtkwmozkze.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cheryme.top/gtiglmusao.html

Ruby: puts "Hello, World!"
来源：http://hz.wangdashe.top/gthqyogtkt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yanxiufei.cn/gtyjtqcwql.html

[A02] 变量声明与赋值
来源：http://hz.guowangkeji.top/gtcimvodzd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangtech.top/gthkgotphp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shzxlz.cn/gtstpaicwr.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shuidangran.top/gtmdromjgu.html


<!-- 参考信息 -->