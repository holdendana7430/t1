代发 wailian999

[U33] Py：打包发布
来源：http://hz.chenzaomai.com/gtoopaumvs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gtiwgnrgkn.html

[U34] Py：判断编码
来源：http://hz.jlsjyb.cn/gtfluzxwaj.html

chardet.detect(raw)
来源：http://hz.guannengcc.top/gtiwlrxgaf.html

[U35] Py：发送邮件
来源：http://hz.hammf.cn/gtuogahlsq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.52xcode.cn/gtaqhfmdyo.html

[U36] Py：定时任务
来源：http://hz.daria6918.cn/gtjckmplhb.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gtasklhriy.html

[U37] Py：读写 Excel
来源：http://hz.yuxming.cn/gtvyokadiw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydzc1.top/gtbiggtrur.html

[U38] Py：获取脚本所在目录
来源：http://hz.tianlin.xyz/gtzieracjx.html

Path(__file__).resolve().parent
来源：http://hz.zhiwuduotai.top/gtepbrswhc.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhiwuduotai.top/gtoufzjpoz.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtusjbgfpb.html

[U40] Py：打印到标准错误
来源：http://hz.jqgfzy.top/gtmltjpwsj.html

print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtdpzjhnxi.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ppjwa.cn/gtkoflilbz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yj20258.top/gtyltgjysw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuanzx.com/gtgbjxqlmp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zdqjudy.top/gtpvjikkiq.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangkeji.top/gthetgohuq.html

namespace App\Http;
来源：http://hz.feifeiyinyue.top/gtvxbemckm.html

[U44] PHP：开启严格类型
来源：http://hz.mhx1999.top/gtzwcodvbq.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gtbhbuijmi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhiwuduotai.top/gtcdxuxvat.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtbinnqpuv.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtldtrpfom.html

?string $name = null
来源：http://hz.dashuyun.cn/gtvntlvaeo.html

[U47] PHP：联合类型
来源：http://hz.andypj.xyz/gtffastmzo.html

int|string $id
来源：http://hz.ehwqpu.com/gtokuhimou.html

[U48] PHP：纯枚举
来源：http://hz.ivvv.top/gtfofhghmt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj202588.top/gtzqvyrotc.html

[U49] PHP：只读属性
来源：http://hz.9152youxi.cn/gticpcngjc.html

public readonly string $name
来源：http://hz.guannengcc.top/gtwnypswai.html

[U50] PHP：构造器属性提升
来源：http://hz.nwbrower.top/gtknfjobsk.html

public function __construct(private int $id) {}
来源：http://hz.yuanzhike.top/gtnbflzmpd.html

[U51] PHP：数组解构
来源：http://hz.jinqigufen.top/gtgtlcbnjf.html

[$a, $b] = $arr;
来源：http://hz.shangyingyoupin.top/gtpgrgivos.html

[U52] PHP：箭头函数
来源：http://hz.xylfe.cn/gtnebvgeqo.html

$double = fn($x) => $x * 2;
来源：http://hz.hongshengwenyu.top/gtcixhcruv.html

[U53] PHP：空合并运算符
来源：http://hz.cheryme.top/gtwjnglrht.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangtech.top/gtwgdsiqyk.html

[U54] PHP：空安全调用
来源：http://hz.xylfe.cn/gtlffwvlnc.html

$obj?->method()
来源：http://hz.daria6918.cn/gtairclqsd.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtfpofrmkc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gttsqirpvi.html

[U56] PHP：命名参数
来源：http://hz.tanke756.top/gtoqwlfjdr.html

f(a: 1, b: 2)
来源：http://hz.pycfn.com/gtkvvdvnha.html

[U57] PHP：字符串插值
来源：http://hz.wangdashe.top/gtactwuijn.html

"值: {$a}"
来源：http://hz.sufxvd.cn/gtqdzdjhrm.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtfyiwliva.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zycfv.cn/gtsrocawyf.html

[U59] PHP：自定义排序
来源：http://hz.zhijiandao.cn/gtlyfbnyef.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtgfyrtwyn.html

[U60] PHP：JSON 编解码
来源：http://hz.zhongyouzk.top/gtjtaqjvsd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hongshengwenyu.top/gtpynfciwt.html

[U61] PHP：正则
来源：http://hz.hnqzz.top/gtqhxuqfae.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtwdmmxatq.html

[U62] PHP：日期对象
来源：http://hz.tian-w.cn/gtevcoyrkm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinghuilouyu.cn/gtpoiuaxzr.html

[U63] PHP：文件读写
来源：http://hz.hnqzz.top/gtdgprcdlw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.svipenyu.cn/gtnfmfsbyd.html

[U64] PHP：目录遍历
来源：http://hz.yuanzhike.top/gtdeczdgft.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtqdtsqkpz.html

[U65] PHP：会话
来源：http://hz.snrcjt.cn/gtrrppwjnh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jqgfzy.top/gtffypajxo.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gthqiizwks.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.52xcode.cn/gtqfpfjppv.html

[U67] PHP：处理文件上传
来源：http://hz.redwolf501.top/gtognrbqdk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hysaishi.cn/gtqystbkjw.html

[U68] PHP：PDO 连接
来源：http://hz.yj202588.top/gtzzipftsy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenlongwang.top/gtkcaofsyk.html

[U69] PHP：PDO 预处理
来源：http://hz.9152youxi.cn/gtpnxnztxw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.fengsongda.top/gtuvkoxugt.html

[U70] PHP：PDO 事务
来源：http://hz.sweek.top/gthsewgasq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yongpay.top/gtdqmyipev.html

[U71] PHP：抛出异常
来源：http://hz.jianghu66.top/gtwujytpet.html

throw new RuntimeException("失败", 500);
来源：http://hz.sweek.top/gtlomlpeov.html

[U72] PHP：写错误日志
来源：http://hz.gaohongyu789.top/gttxmyfvnd.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yangfankeji.com/gtpvlxloun.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtlxpahqlb.html

parse_ini_file("config.ini", true)
来源：http://hz.kuanghao11.cn/gtjxdnfcus.html

[U74] PHP：读取环境变量
来源：http://hz.ivvv.top/gtoufbxomn.html

getenv("APP_ENV") ?: "production"
来源：http://hz.haohaochexian.top/gtfhjslubo.html

[U75] PHP：依赖注入
来源：http://hz.ydzc1.top/gtldgzukel.html

composer require psr/container
来源：http://hz.52xcode.cn/gtnifiwfcu.html

[U76] PHP：简单路由
来源：http://hz.yongpay.top/gtaqbooldq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xziqi.cn/gtihxlutwl.html

[U77] PHP：模板渲染
来源：http://hz.0kj1m.cn/gttayrgatp.html

composer require twig/twig
来源：http://hz.ppjwa.cn/gtshcusgcl.html

[U78] PHP：单元测试
来源：http://hz.guannengcc.top/gtmvtxciyl.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigfzy.top/gtzlmcfpfn.html

[U79] PHP：静态分析
来源：http://hz.chenlongwang.top/gtnpasoest.html

composer require --dev phpstan/phpstan
来源：http://hz.cucudq.cn/gttawaxcal.html

[U80] PHP：代码规范修复
来源：http://hz.cqqwz.cn/gtgnupeorh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtuyxrjzkd.html

[U81] JS：初始化项目
来源：http://hz.cashguo.top/gtfajtdnao.html

npm init -y;  npm i express
来源：http://hz.zhoulong.xyz/gtlclnssxe.html

[U82] JS：package.json 脚本
来源：http://hz.pycfn.com/gthnxttwkc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hnqzz.top/gtojhjvbyp.html

[U83] JS：ES Module 导入导出
来源：http://hz.aibaodan.cn/gtyhplebqn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jinqigfzy.top/gtifegucjg.html

[U84] JS：CommonJS 写法
来源：http://hz.zhoulong.xyz/gtugxlxolq.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.cqqwz.cn/gtdeuunsgs.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtjoworvmm.html

a?.b?.c
来源：http://hz.yanxiufei.cn/gtqvqrnamx.html

[U86] JS：空值合并
来源：http://hz.quarkkingdee.top/gtiyetvlxe.html

a ?? b
来源：http://hz.shanyushiyangtech.top/gtzeareqzn.html

[U87] JS：解构默认值
来源：http://hz.zhongyouzk.top/gtrzzkmcym.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yueranfly.top/gtuwthzkgd.html

[U88] JS：对象展开合并
来源：http://hz.zhengqikj.top/gtxkusorts.html

{ ...a, ...b }
来源：http://hz.hongshengwenyu.top/gtybhqczkl.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gtmzgwhfpv.html

[...new Set(arr)]
来源：http://hz.chenlongwang.top/gtrgqqtmwp.html

[U90] JS：数字数组排序
来源：http://hz.hnxiangtu.top/gtfzgtkang.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtukzvnaml.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gtzthajahr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ppjwa.cn/gtoheoevpk.html

[U92] JS：深拷贝
来源：http://hz.cucudq.cn/gtyvciiqia.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtcyhfgktm.html

[U93] JS：模板字符串
来源：http://hz.sweek.top/gtpzutwiaq.html

`共 ${n} 条`
来源：http://hz.daria6918.cn/gtmjhqwpyi.html

[U94] JS：箭头函数
来源：http://hz.zhongyouzk.top/gtnacmwptw.html

const double = x => x * 2;
来源：http://hz.gogol.net.cn/gtazecpuuv.html

[U95] JS：Promise 包装
来源：http://hz.ywan-chungtsiang.top/gthnrgaywi.html

new Promise((resolve, reject) => {})
来源：http://hz.nwbrower.top/gtcbvmoonr.html

[U96] JS：async/await 与异常
来源：http://hz.xingfuxueyuan.xyz/gtadxbkjku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtzhzevlgb.html

[U97] JS：并发请求
来源：http://hz.yvedp.cn/gtksshiqcl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtoxmcbnqd.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhongyouzk.top/gtwohdgnxb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhoulong.xyz/gtuggzulqn.html

[U99] JS：事件监听
来源：http://hz.yuanzhike.top/gtzswmfpbl.html

el.addEventListener("click", e => {})
来源：http://hz.fengsongda.top/gtfvkqleol.html

[U100] JS：DOM 查询
来源：http://hz.cashguo.top/gtdbekwdgz.html

document.querySelector(".item")
来源：http://hz.yj202588.top/gtzaxhsydl.html

[U101] JS：classList 操作
来源：http://hz.jinyuanbaomall.cn/gtweeporvk.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gtxlkkvjcv.html

[U102] JS：本地存储
来源：http://hz.dashuyun.cn/gtxnsfirde.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hfpthk.cn/gtgpbihgdx.html

[U103] JS：定时器
来源：http://hz.zhongyouzk.top/gtoitqstyo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yonumen.top/gtgdoijzjv.html

[U104] JS：防抖
来源：http://hz.dashuyun.cn/gtkilfblqp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtrtxayeag.html

[U105] JS：节流
来源：http://hz.xziqi.cn/gtwbedibrq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daria6918.cn/gtycdfqsik.html

[U106] JS：日期格式化
来源：http://hz.shzxlz.cn/gtcbpffgzo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangkeji.top/gtxtduisor.html

[U107] JS：数字千分位
来源：http://hz.yonumen.top/gttysohuer.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xinyue.icu/gtyqjescfp.html

[U108] JS：随机整数
来源：http://hz.ywan-chungtsiang.top/gtjnbmtouh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.bjfxy.top/gtfwrguoqp.html

[U109] JS：数组分组
来源：http://hz.redwolf501.top/gtktvthwii.html

Object.groupBy(arr, x => x.type)
来源：http://hz.dianchejie.cn/gtliwcdrzt.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gtqcujeiuq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuetiantiany.cn/gthkjefeyu.html

[U111] JS：对象转 Map
来源：http://hz.0kj1m.cn/gtzubhpbts.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gtirvnqdxv.html

[U112] JS：字符串补位
来源：http://hz.jyoumei.cn/gtoreysgle.html

"7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtvxlznuek.html

[U113] JS：正则替换全部
来源：http://hz.xylfe.cn/gtrncnzqux.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtvjwrddvt.html

[U114] JS：JSON 深比较
来源：http://hz.chenzaomai.com/gthrdexmft.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtzxdbxjfq.html

[U115] JS：生成 UUID
来源：http://hz.andypj.xyz/gtywusrejf.html

crypto.randomUUID()
来源：http://hz.jianghu66.top/gtlxvmledg.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhongyouzk.top/gtofyqttqp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuetiantiany.cn/gtffljnwwi.html

[U117] JS：单元测试
来源：http://hz.hfpthk.cn/gtaxnymutj.html

npm i -D vitest;  npx vitest
来源：http://hz.shanyushiyangtech.top/gtwbcraafk.html

[U118] JS：开发服务器
来源：http://hz.ppjwa.cn/gtujvbcadw.html

npm i -D vite;  npx vite
来源：http://hz.svipenyu.cn/gtayycpyqd.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangtech.top/gtwllcvmoh.html

npx vite build
来源：http://hz.hywenlv.cn/gtkyjblmvp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtxqxjwolr.html

import.meta.env.VITE_API_URL
来源：http://hz.jinyuanbaomall.cn/gthjndqkvw.html

================================================================================
来源：http://hz.fengsongda.top/gtstoeulea.html

统计汇总
来源：http://hz.yangfankeji.com/gtoyncsynf.html

================================================================================
来源：http://hz.cqqwz.cn/gtgyzqebql.html

按语言统计（条）：
来源：http://hz.cashguo.top/gtyddqhhij.html

Python ......... 252
来源：http://hz.hammf.cn/gtotgofwzl.html

PHP ............ 252
来源：http://hz.wangdashe.top/gthrbafroy.html

JavaScript ..... 252
来源：http://hz.havefunace.top/gtznsslwsy.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtfqnklaos.html

Java ........... 212
来源：http://hz.aizwys.cn/gtyimqrexy.html

Go ............. 212
来源：http://hz.iojbl.cn/gtfqqwgjwh.html

Ruby ........... 212
来源：http://hz.ehwqpu.com/gtuvqthagk.html

C# ............. 212
来源：http://hz.hysaishi.cn/gtfcnpljbi.html

C .............. 30
来源：http://hz.ybcxt.top/gttecqdumy.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gtmuqpsxhg.html

SQL ............ 90
来源：http://hz.havefunace.top/gtcecagfvs.html

Bash ........... 80
来源：http://hz.cheryme.top/gtvbjcrkjf.html

Kotlin ......... 15
来源：http://hz.zhoulong.xyz/gtewslcerb.html

Swift .......... 15
来源：http://hz.xingfuxueyuan.xyz/gtgowceaid.html

Lua ............ 10
来源：http://hz.ehwqpu.com/gtvuargyao.html

Perl ........... 10
来源：http://hz.ydjk.org.cn/gtkkrhmwwi.html

Scala .......... 10
来源：http://hz.jinghuilouyu.cn/gtxftvlcuz.html

------------------------------------
来源：http://hz.zycfv.cn/gtconhbywz.html

合计 ........... 2106 条
来源：http://hz.guannengcc.top/gtohebnxia.html

按章节统计：
来源：http://hz.daria6918.cn/gtmjsemazx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shzxlz.cn/gtkjvzvekx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.mhx1999.top/gtxoxnshfl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinqigfzy.top/gtdflqtqjy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtoqesnste.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhaomingkeji.xyz/gtsdejpknf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yvedp.cn/gtfammjvwj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtuhhergdt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtszpvftht.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtzglotens.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtgpfftuop.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtfvbuvpbs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtlbjprpea.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtkdapxzpb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ywan-chungtsiang.top/gtnonyxowl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shzxlz.cn/gtomkdyiqb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtrvraubns.html

Q SQL 专题                              90
来源：http://hz.zhixingplan.top/gtgghxmxtc.html

R Bash 专题                             80
来源：http://hz.andypj.xyz/gtgfmpjvxr.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtjrdchjrn.html

T 其他语言补充                          60
来源：http://hz.nanxinkj.top/gtxvaopety.html

U 高频实用片段                         120
来源：http://hz.hysaishi.cn/gtregxpeqz.html

------------------------------------
来源：http://hz.tanke756.top/gtflxmwezi.html

合计                                  2106 条
来源：http://hz.tian-w.cn/gtbtfmkqmu.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gteviitfxa.html

使用提醒
来源：http://hz.hfpthk.cn/gtdydwtysv.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtjvoiwnxi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.sxryk.cn/gtumesaohe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gogol.net.cn/gtojhkdtco.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fengsongda.top/gtqkmioupd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.c1oappe.top/gtuffiysuo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jianghu66.top/gtgoqtezyw.html

—— 文件结束 ——
来源：http://hz.yj20258888.top/gtmapofwye.html

================================================================================
来源：http://hz.snrcjt.cn/gtamlhqrma.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hfpthk.cn/gtkmnqdcib.html

Common Programming Examples Cheat Book
来源：http://hz.kuanghao11.cn/gttrmecnju.html

================================================================================
来源：http://hz.yj20258.top/gtrdqwjhth.html

【收录内容】
来源：http://hz.jyoumei.cn/gtjzhobsen.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.chenzaomai.com/gtdldzymud.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuxming.cn/gtjhixegpe.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gtxzcfjgce.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.xuanzx.com/gtlpdfbzta.html

【使用说明】
来源：http://hz.yj20258.top/gtrzvntdmx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.quarkkingdee.top/gthttrqhnm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258888.top/gtdoqzdigq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cqqwz.cn/gtjoragykn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.pycfn.com/gtsxwshzqo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.svipenyu.cn/gtogedzagm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj20258888.top/gtsxwathbj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhaomingkeji.xyz/gtmahefhso.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.zhongyouzk.top/gtqsyiiwha.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.iojbl.cn/gtdtuwpjlg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.gotoacloud.top/gtlzshqjrz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtpfowhvuc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.gogol.net.cn/gtuariltnb.html

【文件统计】
来源：http://hz.feifeiyinyue.top/gtowdnhorl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.fzhhl.top/gtckhckqug.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtslikenng.html

目  录
来源：http://hz.hongshengwenyu.top/gtwcdblwtp.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtbmkcleio.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.dianchejie.cn/gtigvaktit.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gteqfuvkdq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xingfuxueyuan.xyz/gtylzasvds.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtypofihyc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.cashguo.top/gtmqagxnsy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gtbatzbnqb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtekocgybg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.snrcjt.cn/gtwuqsifaq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtskykgryc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.haohaochexian.top/gtpuxlsbsp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtgvkilkxm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtlzstdgmb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtaswiooxn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtcwbobhsq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ydjk.org.cn/gtujtqmaho.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtwiggsthg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtqgyzerfr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shuidangran.top/gtzstqsfaf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgfzy.top/gtywvshdrc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtxzpwofrv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtqxdqwkev.html

================================================================================
来源：http://hz.sysykeji.top/gtkikbsrip.html

A. 基础语法与类型
来源：http://hz.jqgufenzy.top/gtailavyjw.html

================================================================================
来源：http://hz.xuanzx.com/gtjkbhsjlm.html

[A01] Hello World
来源：http://hz.dianchejie.cn/gtmnbxiyly.html

Py:   print("Hello, World!")
来源：http://hz.havefunace.top/gtyzaamiwn.html

PHP:  echo "Hello, World!";
来源：http://hz.gzhubu.top/gtygptxnkn.html

JS:   console.log("Hello, World!");
来源：http://hz.mhx1999.top/gtlehbnbqe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yongpay.top/gtwihkoclk.html

Java: System.out.println("Hello, World!");
来源：http://hz.hammf.cn/gtqzlivhds.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.vqdsnc.cn/gtztnjvhok.html

Ruby: puts "Hello, World!"
来源：http://hz.ydjk.org.cn/gtyiqvrykz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.snrcjt.cn/gtdsahnbxc.html

[A02] 变量声明与赋值
来源：http://hz.zdqjudy.top/gtbzwhvdmt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.mhx1999.top/gtlfoxpbla.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.fengsongda.top/gtrpdqbjjz.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gaohongyu789.top/gtdrtgxtuo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.cdnleiting.top/gttlxaybaf.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gttsjlclav.html

Go:   name := "Alex"; age := 20
来源：http://hz.fzhhl.top/gtpuzydzdg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.guowangkeji.top/gtstmwdwix.html


<!-- 参考信息 -->