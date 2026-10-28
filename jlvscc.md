代发 wailian999

[U33] Py：打包发布
来源：http://hz.zhongyouzk.top/gteahaglma.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gtwxbyinty.html

[U34] Py：判断编码
来源：http://hz.chenlongwang.top/gtifvylola.html

chardet.detect(raw)
来源：http://hz.andypj.xyz/gtxtrrnkxq.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtqfowwsjq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtzliwggll.html

[U36] Py：定时任务
来源：http://hz.hongshengwenyu.top/gtlebercuk.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtswxixkgm.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtuwpfoysq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenjidiqi.icu/gtugqsgmeo.html

[U38] Py：获取脚本所在目录
来源：http://hz.shanyushiyangtech.top/gtousbwknd.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtxvgvnwko.html

[U39] Py：判断是否在交互环境
来源：http://hz.havefunace.top/gteciipafr.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtfjxoqyfn.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gttxmckuhq.html

print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtxzelavqx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guowangkeji.top/gtzjfuccln.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhengqikj.top/gthvwsdoyp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hfpthk.cn/gtxrxlpupr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenzaomai.com/gtoehjldtv.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gtbtdzwjio.html

namespace App\Http;
来源：http://hz.hammf.cn/gtyzzfsavi.html

[U44] PHP：开启严格类型
来源：http://hz.daria6918.cn/gtadmavdra.html

declare(strict_types=1);
来源：http://hz.xingfuxueyuan.xyz/gtrsmglmfi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtkifzisqx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtttgypegx.html

[U46] PHP：可空类型
来源：http://hz.hammf.cn/gtgehlfxjy.html

?string $name = null
来源：http://hz.yueranfly.top/gtttmhxlyw.html

[U47] PHP：联合类型
来源：http://hz.yonumen.top/gtbvbgyopx.html

int|string $id
来源：http://hz.0kj1m.cn/gtfjlgsipq.html

[U48] PHP：纯枚举
来源：http://hz.feifeiyinyue.top/gtutrclihj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtqplhxzre.html

[U49] PHP：只读属性
来源：http://hz.jyoumei.cn/gtaqwvimxn.html

public readonly string $name
来源：http://hz.sweek.top/gtqfyqeirs.html

[U50] PHP：构造器属性提升
来源：http://hz.vqdsnc.cn/gtovqianoh.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtiooxtbco.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtazwphezv.html

[$a, $b] = $arr;
来源：http://hz.yj20258.top/gtgvfslcyc.html

[U52] PHP：箭头函数
来源：http://hz.chenlongwang.top/gtctgjittj.html

$double = fn($x) => $x * 2;
来源：http://hz.hnxiangtu.top/gtjknqdinx.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gtjejfnfcw.html

$v = $a ?? $b ?? "default";
来源：http://hz.yuanzhike.top/gtwevwwlld.html

[U54] PHP：空安全调用
来源：http://hz.hfpthk.cn/gtmvqlbpgs.html

$obj?->method()
来源：http://hz.iojbl.cn/gtnepwsjwx.html

[U55] PHP：match 表达式
来源：http://hz.gzhubu.top/gtkaiwwzaj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cashguo.top/gtoyyzfwyx.html

[U56] PHP：命名参数
来源：http://hz.cdnleiting.top/gtiozrylok.html

f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtezoztcvi.html

[U57] PHP：字符串插值
来源：http://hz.wangshuangyany.cn/gttgcxcqun.html

"值: {$a}"
来源：http://hz.yj202588.top/gtyeslmtzt.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtfotjcugd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gzhubu.top/gtvoemquhy.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtowrbgmdx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtmkubeonn.html

[U60] PHP：JSON 编解码
来源：http://hz.yuxming.cn/gtajjqqhaz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gtxmslitzz.html

[U61] PHP：正则
来源：http://hz.mhx1999.top/gtahhttjfl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtddqeqhin.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtuujzkfzs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jlsjyb.cn/gtaphvqnge.html

[U63] PHP：文件读写
来源：http://hz.andypj.xyz/gtkpdmbfrx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuetiantiany.cn/gtbaurplfn.html

[U64] PHP：目录遍历
来源：http://hz.wangdashe.top/gtolgyxggn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtmdjqzgsw.html

[U65] PHP：会话
来源：http://hz.chenzaomai.com/gtnzdnwmtg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pycfn.com/gticowqfjz.html

[U66] PHP：设置 Cookie
来源：http://hz.iojbl.cn/gtczmefcrz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nanxuanxn.top/gtgpoiecob.html

[U67] PHP：处理文件上传
来源：http://hz.shanyushiyangtech.top/gtifvlgeoe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.wangdashe.top/gtzivbebaq.html

[U68] PHP：PDO 连接
来源：http://hz.quarkkingdee.top/gtsytykzqd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gthybgmmtt.html

[U69] PHP：PDO 预处理
来源：http://hz.birdmap.top/gttlmpcvxg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hfpthk.cn/gtkcezfuxt.html

[U70] PHP：PDO 事务
来源：http://hz.xuanzx.com/gtcktohadp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgfzy.top/gtpgafsoqp.html

[U71] PHP：抛出异常
来源：http://hz.shangyingyoupin.top/gtztluiblh.html

throw new RuntimeException("失败", 500);
来源：http://hz.mhx1999.top/gtdkzrcdxs.html

[U72] PHP：写错误日志
来源：http://hz.yj20258.top/gttehrhcch.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yuxming.cn/gtnsyedrml.html

[U73] PHP：读取 ini 配置
来源：http://hz.yongpay.top/gtmjzvlskw.html

parse_ini_file("config.ini", true)
来源：http://hz.bjfxy.top/gtfswznrpr.html

[U74] PHP：读取环境变量
来源：http://hz.snrcjt.cn/gtspjufkwk.html

getenv("APP_ENV") ?: "production"
来源：http://hz.haohaochexian.top/gtaijyqzyj.html

[U75] PHP：依赖注入
来源：http://hz.daria6918.cn/gtfldrcvjl.html

composer require psr/container
来源：http://hz.jianghu66.top/gtgkvcuxtc.html

[U76] PHP：简单路由
来源：http://hz.gzhubu.top/gtnxatugcx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtnmqgowsy.html

[U77] PHP：模板渲染
来源：http://hz.snrcjt.cn/gtaatqitze.html

composer require twig/twig
来源：http://hz.cashguo.top/gtjltjakzz.html

[U78] PHP：单元测试
来源：http://hz.gotoacloud.top/gtgpcvmvof.html

composer require --dev phpunit/phpunit
来源：http://hz.tian-w.cn/gtxcreikrz.html

[U79] PHP：静态分析
来源：http://hz.yonumen.top/gtylllzqxh.html

composer require --dev phpstan/phpstan
来源：http://hz.vqdsnc.cn/gtwxuqwkjs.html

[U80] PHP：代码规范修复
来源：http://hz.jqgufenzy.top/gtfjoaoqhc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigfzy.top/gtntdheivd.html

[U81] JS：初始化项目
来源：http://hz.quarkkingdee.top/gtrvrhjcmh.html

npm init -y;  npm i express
来源：http://hz.yongpay.top/gtnklghnxp.html

[U82] JS：package.json 脚本
来源：http://hz.ppjwa.cn/gtmhjzjozd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jiagoushi.top/gthrxhzdlw.html

[U83] JS：ES Module 导入导出
来源：http://hz.fengsongda.top/gtjkeuwmse.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.gotoacloud.top/gtkycdlmrv.html

[U84] JS：CommonJS 写法
来源：http://hz.jinyuanbaomall.cn/gtzgdodriv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yanxiufei.cn/gtmjpmqiio.html

[U85] JS：可选链
来源：http://hz.guannengcc.top/gtpdkwbbac.html

a?.b?.c
来源：http://hz.yonumen.top/gtjsdmmkje.html

[U86] JS：空值合并
来源：http://hz.bjfxy.top/gteguihvvt.html

a ?? b
来源：http://hz.birdmap.top/gtewwgjvli.html

[U87] JS：解构默认值
来源：http://hz.52xcode.cn/gtomfqfmpa.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zdqjudy.top/gtnkyhknrl.html

[U88] JS：对象展开合并
来源：http://hz.yanxiufei.cn/gtobantgry.html

{ ...a, ...b }
来源：http://hz.shanyushiyangkeji.top/gtqtztisbd.html

[U89] JS：数组去重
来源：http://hz.ydjk.org.cn/gtmpecqugx.html

[...new Set(arr)]
来源：http://hz.jinqigufen.top/gtzcdliben.html

[U90] JS：数字数组排序
来源：http://hz.jinyuanbaomall.cn/gtoegzqjdi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtfgpjajfl.html

[U91] JS：对象键值遍历
来源：http://hz.jinghuilouyu.cn/gtwrgygujz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.52xcode.cn/gtwpanpuvu.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gttclnjveg.html

structuredClone(obj)
来源：http://hz.sufxvd.cn/gtqbcluayb.html

[U93] JS：模板字符串
来源：http://hz.gotoacloud.top/gtrbcdjjab.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtukduorgr.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtqipohxlx.html

const double = x => x * 2;
来源：http://hz.xinyue.icu/gtmonbeygl.html

[U95] JS：Promise 包装
来源：http://hz.yanxiufei.cn/gtxbsngspk.html

new Promise((resolve, reject) => {})
来源：http://hz.tanke756.top/gtegvbguya.html

[U96] JS：async/await 与异常
来源：http://hz.xuanzx.com/gtvtgdioul.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtzoxcszbo.html

[U97] JS：并发请求
来源：http://hz.yuxming.cn/gthedztrnm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtknpaasxi.html

[U98] JS：fetch 带 JSON
来源：http://hz.jlsjyb.cn/gtjhbscuyq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xylfe.cn/gtnhymlwyi.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtavqtdjsw.html

el.addEventListener("click", e => {})
来源：http://hz.chenzaomai.com/gtvmtkvkql.html

[U100] JS：DOM 查询
来源：http://hz.cucudq.cn/gtkyqgcxwy.html

document.querySelector(".item")
来源：http://hz.sweek.top/gtqkpkkswm.html

[U101] JS：classList 操作
来源：http://hz.bjfxy.top/gtinxxraxw.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtycmbrfdy.html

[U102] JS：本地存储
来源：http://hz.gotoacloud.top/gtspxvoscs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.9152youxi.cn/gtzmjilaub.html

[U103] JS：定时器
来源：http://hz.xziqi.cn/gtkgkdrffi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gteinmtpkc.html

[U104] JS：防抖
来源：http://hz.xylfe.cn/gtazlenfnw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtctrzwdwo.html

[U105] JS：节流
来源：http://hz.cheryme.top/gtkrgkalqd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.feifeiyinyue.top/gtrmyzbduh.html

[U106] JS：日期格式化
来源：http://hz.fengsongda.top/gtyigqnlnu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.cheryme.top/gtnnjrhkpl.html

[U107] JS：数字千分位
来源：http://hz.ppjwa.cn/gtorxuiuaj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cucudq.cn/gtkyqowypy.html

[U108] JS：随机整数
来源：http://hz.jiagoushi.top/gtpzmjskyc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.52xcode.cn/gtgwocfniy.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtauxvgond.html

Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtliakcsob.html

[U110] JS：数组分块
来源：http://hz.jyoumei.cn/gtfwbatoud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.c1oappe.top/gtuqyeruel.html

[U111] JS：对象转 Map
来源：http://hz.wangshuangyany.cn/gtdzpgwutq.html

new Map(Object.entries(obj))
来源：http://hz.52xcode.cn/gtxmtllpvs.html

[U112] JS：字符串补位
来源：http://hz.pengpengdd.cyou/gtzyiyyxjj.html

"7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtduchmnlm.html

[U113] JS：正则替换全部
来源：http://hz.ydjk.org.cn/gtqlsetkqb.html

s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gthbfnkyde.html

[U114] JS：JSON 深比较
来源：http://hz.daxiang520.top/gtqxokwzif.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtjymember.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtteozqkuu.html

crypto.randomUUID()
来源：http://hz.shuidangran.top/gteaboiuir.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhengqikj.top/gteeevxiuo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yongpay.top/gthjfyzrfj.html

[U117] JS：单元测试
来源：http://hz.redwolf501.top/gtaalpooow.html

npm i -D vitest;  npx vitest
来源：http://hz.nwbrower.top/gtbtgnotnc.html

[U118] JS：开发服务器
来源：http://hz.cdnleiting.top/gtztujuzvc.html

npm i -D vite;  npx vite
来源：http://hz.hongshengwenyu.top/gtmxsegozv.html

[U119] JS：生产构建
来源：http://hz.52xcode.cn/gtksjwlghn.html

npx vite build
来源：http://hz.snrcjt.cn/gtwmjynrvl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtuqagrool.html

import.meta.env.VITE_API_URL
来源：http://hz.smart0.xyz/gtcohqpqif.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpzlesbkx.html

统计汇总
来源：http://hz.aizwys.cn/gtbtpnoivf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwejrrjve.html

按语言统计（条）：
来源：http://hz.0kj1m.cn/gttrqqziua.html

Python ......... 252
来源：http://hz.jiagoushi.top/gtmferfkeo.html

PHP ............ 252
来源：http://hz.zycfv.cn/gtwwgbasiu.html

JavaScript ..... 252
来源：http://hz.bjfxy.top/gtxypfdwuv.html

TypeScript ..... 212
来源：http://hz.andypj.xyz/gtanwbwcfg.html

Java ........... 212
来源：http://hz.zycfv.cn/gthhfdfjvk.html

Go ............. 212
来源：http://hz.birdmap.top/gtuafofies.html

Ruby ........... 212
来源：http://hz.pycfn.com/gtazzqirgx.html

C# ............. 212
来源：http://hz.xziqi.cn/gtfwcwgmzy.html

C .............. 30
来源：http://hz.jinyuanbaomall.cn/gtktfvhxfi.html

C++ ............ 30
来源：http://hz.jianghu66.top/gtpojehcpq.html

SQL ............ 90
来源：http://hz.yangfankeji.com/gtpkizfadq.html

Bash ........... 80
来源：http://hz.wangdashe.top/gttzulgvjq.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtantehsli.html

Swift .......... 15
来源：http://hz.cucudq.cn/gtofnepqoc.html

Lua ............ 10
来源：http://hz.meibo888.top/gtoomobika.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtrnyxhdxx.html

Scala .......... 10
来源：http://hz.meibo888.top/gtyllxbdjo.html

------------------------------------
来源：http://hz.tianlin.xyz/gtjrvqvroi.html

合计 ........... 2106 条
来源：http://hz.shanyushiyangtech.top/gtwxfvfsgb.html

按章节统计：
来源：http://hz.jqgfzy.top/gtinebdabq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.bjfxy.top/gtxhtnicee.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.shangyingyoupin.top/gtqfrsjrrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtdapoibzz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yonumen.top/gtkslkzojt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ivvv.top/gtavwzqvri.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtzjoujusw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gtbbxmpkgr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtxkcxtayv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zdqjudy.top/gtlgnmbjpo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtjqrkxqpp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtkzivufkn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinghuilouyu.cn/gtrflyghyc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtmrudgjaz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtowviuddu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cheryme.top/gtexkppago.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtuxzccxad.html

Q SQL 专题                              90
来源：http://hz.jyoumei.cn/gtbtzqpavq.html

R Bash 专题                             80
来源：http://hz.jinqigufen.top/gthzvuphyf.html

S C / C++ 专题                          60
来源：http://hz.gogol.net.cn/gttpvneqyg.html

T 其他语言补充                          60
来源：http://hz.hnxiangtu.top/gtsfwapgym.html

U 高频实用片段                         120
来源：http://hz.bjfxy.top/gttvvkzioe.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtzzusvyel.html

合计                                  2106 条
来源：http://hz.jianghu66.top/gtztyjlgvz.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtbqciyxfu.html

使用提醒
来源：http://hz.daria6918.cn/gtyofsxici.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtlchptgoe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ivvv.top/gtiynbjfme.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.quarkkingdee.top/gtkpoepqce.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yueranfly.top/gtmsbslggj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinyuanbaomall.cn/gtbaqakvso.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.xingfuxueyuan.xyz/gtakrvffuf.html

—— 文件结束 ——
来源：http://hz.jinqigufen.top/gtweutswiq.html

================================================================================
来源：http://hz.cdnleiting.top/gtisgxvnbz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ybcxt.top/gtgbroopjb.html

Common Programming Examples Cheat Book
来源：http://hz.sufxvd.cn/gtpbtlcedv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcjufpbhs.html

【收录内容】
来源：http://hz.kuanghao11.cn/gtjdqpakvy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinyuanbaomall.cn/gtvwxfybfs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.haohaochexian.top/gtylcjqqlv.html

SQL · Bash · C · C++
来源：http://hz.hywenlv.cn/gtvatkbsdo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.mhx1999.top/gtyhqmlsyz.html

【使用说明】
来源：http://hz.hammf.cn/gtucmyyelq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xuetiantiany.cn/gtgnhfjdam.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.guowangkeji.top/gtjiggirtp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.svipenyu.cn/gtzcovwlim.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ehwqpu.com/gtuodvrlbp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.redwolf501.top/gtaogivquo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shuidangran.top/gtyqwzwznc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtgvxjovwb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.xuanzx.com/gtncksljbh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hongshengwenyu.top/gttscdsdbz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nanxinkj.top/gtipoxacpj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhixingplan.top/gturfpfdma.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yangfankeji.com/gtjmvodqej.html

【文件统计】
来源：http://hz.vqdsnc.cn/gtfpfmwbpw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.xziqi.cn/gtaqdhbkvu.html

--------------------------------------------------------------------------------
来源：http://hz.xuanzx.com/gtkmbocqvy.html

目  录
来源：http://hz.bjfxy.top/gtmcztbufa.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtbzcohkvr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zdqjudy.top/gtflljrspo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nwbrower.top/gtivntgkns.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenjidiqi.icu/gtgzyucfrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hywenlv.cn/gtmrsqbnvt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hywenlv.cn/gttymgpxdc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnxiangtu.top/gtreimnkbs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jqgfzy.top/gtvlvhsuuq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtpgscknhg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hysaishi.cn/gtufvrvgkf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jyoumei.cn/gtwzoizfks.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtjqoclnik.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtxtrgnczh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtjopzcucw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jyoumei.cn/gtxfjuszdc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fengsongda.top/gtfajhbbzs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtwowstxea.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xuanzx.com/gtduuavhwd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cucudq.cn/gttatwdypo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.pengpengdd.cyou/gtgomfrofu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtznpjwfhg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtcxtninyp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtocslwwwo.html

A. 基础语法与类型
来源：http://hz.guannengcc.top/gtkqopbqyi.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtawpiwhib.html

[A01] Hello World
来源：http://hz.nwbrower.top/gtoybcfzwh.html

Py:   print("Hello, World!")
来源：http://hz.pengpengdd.cyou/gtlzkmswcb.html

PHP:  echo "Hello, World!";
来源：http://hz.xinyue.icu/gtxqsiyuqr.html

JS:   console.log("Hello, World!");
来源：http://hz.redwolf501.top/gtafsklhox.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.chenjidiqi.icu/gtuxjbglol.html

Java: System.out.println("Hello, World!");
来源：http://hz.bjfxy.top/gtgkkwjass.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydzc1.top/gtelnffhbj.html

Ruby: puts "Hello, World!"
来源：http://hz.nanxuanxn.top/gtismnacuy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtohqhbskz.html

[A02] 变量声明与赋值
来源：http://hz.yj20258.top/gtgzsesuoc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yuxming.cn/gtobypztem.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shuidangran.top/gtbdzdcnxx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shzxlz.cn/gtlxoqrqmh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jianghu66.top/gtzbytsiqc.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.iojbl.cn/gthqjbsins.html

Go:   name := "Alex"; age := 20
来源：http://hz.cdnleiting.top/gtlyveoave.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ivvv.top/gtzplmgpxw.html


<!-- 参考信息 -->