代发 wailian999

[U19] Py：正则替换带回调
来源：http://hz.shangyingyoupin.top/gtyiqdxwzo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenzaomai.com/gtayrsoomo.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtpjnzfqky.html

@functools.lru_cache(maxsize=None)
来源：http://hz.birdmap.top/gthjthznwz.html

[U21] Py：自定义上下文管理器
来源：http://hz.jyoumei.cn/gtdhrpooxl.html

@contextlib.contextmanager
来源：http://hz.jlsjyb.cn/gtcibnhett.html

[U22] Py：矩阵转置
来源：http://hz.cqqwz.cn/gtmgqilxaq.html

list(zip(*m))
来源：http://hz.wangdashe.top/gtwpallhjw.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258888.top/gtibjwpoph.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cashguo.top/gtrelqcaox.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gtiwfqlrsa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gtlvzjcqch.html

[U25] Py：CSV 按字典读
来源：http://hz.hnxiangtu.top/gtawfvvras.html

csv.DictReader(f)
来源：http://hz.aibaodan.cn/gtmjqmsqhp.html

[U26] Py：并发下载
来源：http://hz.sweek.top/gtwcakgday.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xziqi.cn/gtgwlnvcua.html

[U27] Py：异步 HTTP
来源：http://hz.gaohongyu789.top/gtvyoxocnh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jqgfzy.top/gtuxpkpwth.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtufbbcusv.html

UserId = int
来源：http://hz.jqgfzy.top/gtjeifwrxa.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gtkylcrbvk.html

@property 与 @x.setter 配合
来源：http://hz.jqgfzy.top/gtdkirhlch.html

[U30] Py：数据类
来源：http://hz.gotoacloud.top/gtptehfkve.html

@dataclass(slots=True)
来源：http://hz.jlsjyb.cn/gtwuhmblyg.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gtpblokhbq.html

python -m pytest -q
来源：http://hz.zhiwuduotai.top/gtwcjfdoha.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gteytunfvn.html

ruff format . && ruff check --fix .
来源：http://hz.shanyushiyangtech.top/gttegkqrnk.html

[U33] Py：打包发布
来源：http://hz.fengsongda.top/gtjvmbqoqb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cashguo.top/gtgdwzuacp.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gtqidtewhk.html

chardet.detect(raw)
来源：http://hz.andypj.xyz/gtvrxkgcnf.html

[U35] Py：发送邮件
来源：http://hz.ehwqpu.com/gtzwrejoyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtdbodsvyr.html

[U36] Py：定时任务
来源：http://hz.jqgfzy.top/gtmlwqkjvx.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydjk.org.cn/gtmouuqxlg.html

[U37] Py：读写 Excel
来源：http://hz.birdmap.top/gtcqegawbi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hywenlv.cn/gterqxqjzm.html

[U38] Py：获取脚本所在目录
来源：http://hz.snrcjt.cn/gtunnzzqgr.html

Path(__file__).resolve().parent
来源：http://hz.jinqigfzy.top/gtlilmiqnr.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenjidiqi.icu/gtwgwkxstx.html

sys.stdout.isatty()
来源：http://hz.ivvv.top/gtajnwpfcy.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gtkewpnbfn.html

print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtzagkxhkb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yonumen.top/gtyjyeowfx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.vqdsnc.cn/gtfhwvjjkt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dashuyun.cn/gtrhmjqthl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nanxinkj.top/gtsspyxxhn.html

[U43] PHP：声明命名空间
来源：http://hz.jianghu66.top/gtsdizrakn.html

namespace App\Http;
来源：http://hz.dashuyun.cn/gtqfalynhz.html

[U44] PHP：开启严格类型
来源：http://hz.wangdashe.top/gtgkxpaejv.html

declare(strict_types=1);
来源：http://hz.shuidangran.top/gtfgsncajv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtebtzrscn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtxferztwm.html

[U46] PHP：可空类型
来源：http://hz.cqqwz.cn/gtqbvzgkjd.html

?string $name = null
来源：http://hz.ehwqpu.com/gthuvzjrtv.html

[U47] PHP：联合类型
来源：http://hz.xziqi.cn/gtfmpkhwzc.html

int|string $id
来源：http://hz.chenlongwang.top/gtfpcezbrt.html

[U48] PHP：纯枚举
来源：http://hz.yanxiufei.cn/gttxpmmazc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydzc1.top/gtggtwrtvo.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtftxipaee.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtuzsbitva.html

[U50] PHP：构造器属性提升
来源：http://hz.xylfe.cn/gtrabdrxov.html

public function __construct(private int $id) {}
来源：http://hz.ehwqpu.com/gternywpko.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtnyyivwzz.html

[$a, $b] = $arr;
来源：http://hz.zhaomingkeji.xyz/gtnarrildj.html

[U52] PHP：箭头函数
来源：http://hz.ybcxt.top/gtwspouicb.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtzbsxsmpw.html

[U53] PHP：空合并运算符
来源：http://hz.gogol.net.cn/gtombqyhbq.html

$v = $a ?? $b ?? "default";
来源：http://hz.hongshengwenyu.top/gtijrrhauo.html

[U54] PHP：空安全调用
来源：http://hz.tanke756.top/gtwjkkwsah.html

$obj?->method()
来源：http://hz.tian-w.cn/gtofsuyueq.html

[U55] PHP：match 表达式
来源：http://hz.kuanghao11.cn/gtulmifdke.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.feifeiyinyue.top/gtdcvxdhpd.html

[U56] PHP：命名参数
来源：http://hz.cucudq.cn/gttpvntdkp.html

f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtvkqrpptv.html

[U57] PHP：字符串插值
来源：http://hz.yongpay.top/gtkygjbrdi.html

"值: {$a}"
来源：http://hz.ydjk.org.cn/gtylwrvjlz.html

[U58] PHP：数组三件套
来源：http://hz.yuxming.cn/gtujesznnz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jqgfzy.top/gtiqnntzjr.html

[U59] PHP：自定义排序
来源：http://hz.tanke756.top/gtuimmcvlg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtdfzzxfbt.html

[U60] PHP：JSON 编解码
来源：http://hz.yangfankeji.com/gtmkuhyiqq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj202588.top/gtxjnqpten.html

[U61] PHP：正则
来源：http://hz.gzhubu.top/gtqnsjllrj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtdlindgyf.html

[U62] PHP：日期对象
来源：http://hz.ehwqpu.com/gtddvpfrnf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinghuilouyu.cn/gtpjizudnj.html

[U63] PHP：文件读写
来源：http://hz.shangyingyoupin.top/gtxefntvtr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aibaodan.cn/gtothmpbaz.html

[U64] PHP：目录遍历
来源：http://hz.gzhubu.top/gtqjnffdhs.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gtgcmfseqq.html

[U65] PHP：会话
来源：http://hz.nanxinkj.top/gtvbiicqff.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dashuyun.cn/gtjpmjrirv.html

[U66] PHP：设置 Cookie
来源：http://hz.jinqigufen.top/gtomqqjxhj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jiagoushi.top/gtknwyhmtx.html

[U67] PHP：处理文件上传
来源：http://hz.zhoulong.xyz/gtanomvjuk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.dianchejie.cn/gtdnzryopr.html

[U68] PHP：PDO 连接
来源：http://hz.jiagoushi.top/gthpqrzxoe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pycfn.com/gtzweajult.html

[U69] PHP：PDO 预处理
来源：http://hz.yj202588.top/gtoslpcsgn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.snrcjt.cn/gttdbmfnch.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtjfithlvs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xinyue.icu/gtafykobdu.html

[U71] PHP：抛出异常
来源：http://hz.jyoumei.cn/gtasetsdjv.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtxcnqmsak.html

[U72] PHP：写错误日志
来源：http://hz.tian-w.cn/gtmijwvxug.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydzc1.top/gtvrapoezf.html

[U73] PHP：读取 ini 配置
来源：http://hz.aizwys.cn/gtetikfvpr.html

parse_ini_file("config.ini", true)
来源：http://hz.yvedp.cn/gtbqvxuasf.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtgxzfuumj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.0kj1m.cn/gtyalpfwig.html

[U75] PHP：依赖注入
来源：http://hz.xuanzx.com/gtttsyfvju.html

composer require psr/container
来源：http://hz.sxryk.cn/gtvhuhvgxy.html

[U76] PHP：简单路由
来源：http://hz.yvedp.cn/gtkbeocmkz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hammf.cn/gtnohncfnf.html

[U77] PHP：模板渲染
来源：http://hz.zycfv.cn/gtjacxehyu.html

composer require twig/twig
来源：http://hz.jianghu66.top/gtqxujydyd.html

[U78] PHP：单元测试
来源：http://hz.fzhhl.top/gtbacziwlf.html

composer require --dev phpunit/phpunit
来源：http://hz.haohaochexian.top/gthbxlhqvv.html

[U79] PHP：静态分析
来源：http://hz.gotoacloud.top/gtpzxxqkkf.html

composer require --dev phpstan/phpstan
来源：http://hz.ybcxt.top/gtqqoaghlw.html

[U80] PHP：代码规范修复
来源：http://hz.redwolf501.top/gtpycayreq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yuanzhike.top/gtdkhrktuy.html

[U81] JS：初始化项目
来源：http://hz.tanke756.top/gtzwjebejm.html

npm init -y;  npm i express
来源：http://hz.yj20258.top/gtcbrbespt.html

[U82] JS：package.json 脚本
来源：http://hz.gogol.net.cn/gtvakbuwcc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtabmhiozm.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gthxnmojbn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtcwgpmzmw.html

[U84] JS：CommonJS 写法
来源：http://hz.jyoumei.cn/gtdoztnnmv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shzxlz.cn/gtmfmtlqvi.html

[U85] JS：可选链
来源：http://hz.zhoulong.xyz/gtvxtkraxh.html

a?.b?.c
来源：http://hz.shangyingyoupin.top/gtggsgqxtg.html

[U86] JS：空值合并
来源：http://hz.yvedp.cn/gtdbaiedgl.html

a ?? b
来源：http://hz.jqgfzy.top/gttbavpjcw.html

[U87] JS：解构默认值
来源：http://hz.yj20258.top/gtsfhuvhwx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenzaomai.com/gtbgxmcikk.html

[U88] JS：对象展开合并
来源：http://hz.ehwqpu.com/gthscluelx.html

{ ...a, ...b }
来源：http://hz.shzxlz.cn/gtfqcanqvs.html

[U89] JS：数组去重
来源：http://hz.smart0.xyz/gtrsjofnlm.html

[...new Set(arr)]
来源：http://hz.316326.xyz/gtuwnhadig.html

[U90] JS：数字数组排序
来源：http://hz.ehwqpu.com/gtokoivfwz.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtlznabozf.html

[U91] JS：对象键值遍历
来源：http://hz.snrcjt.cn/gtcrefsveh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xziqi.cn/gtmcvyjzqv.html

[U92] JS：深拷贝
来源：http://hz.ppjwa.cn/gtjiiumppf.html

structuredClone(obj)
来源：http://hz.mhx1999.top/gttxobqlfq.html

[U93] JS：模板字符串
来源：http://hz.wangshuangyany.cn/gtyjsmblzz.html

`共 ${n} 条`
来源：http://hz.feifeiyinyue.top/gtgdnwaiil.html

[U94] JS：箭头函数
来源：http://hz.cucudq.cn/gteoplmkch.html

const double = x => x * 2;
来源：http://hz.jinghuilouyu.cn/gtatmwvtdw.html

[U95] JS：Promise 包装
来源：http://hz.jyoumei.cn/gtdvtyenot.html

new Promise((resolve, reject) => {})
来源：http://hz.cucudq.cn/gtmhwzpgkl.html

[U96] JS：async/await 与异常
来源：http://hz.sufxvd.cn/gtidqfccph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gthzpqrnqc.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gthbfvjhsu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtauiqbulv.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhiwuduotai.top/gtmedgvzmr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.52xcode.cn/gtswjygptk.html

[U99] JS：事件监听
来源：http://hz.andypj.xyz/gtbehcleld.html

el.addEventListener("click", e => {})
来源：http://hz.hysaishi.cn/gtvyrewdnd.html

[U100] JS：DOM 查询
来源：http://hz.vqdsnc.cn/gtkfbrggkv.html

document.querySelector(".item")
来源：http://hz.yonumen.top/gtxhsotuti.html

[U101] JS：classList 操作
来源：http://hz.mhx1999.top/gtcvlxucsm.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gtvnzgzrpv.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtnmxhwpes.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuxming.cn/gtwhevazdp.html

[U103] JS：定时器
来源：http://hz.hysaishi.cn/gtrouvzipo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shangyingyoupin.top/gtpgtpcrfe.html

[U104] JS：防抖
来源：http://hz.sweek.top/gtujtygrht.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhaomingkeji.xyz/gtlasvylwt.html

[U105] JS：节流
来源：http://hz.yueranfly.top/gtrsyjsszm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhijiandao.cn/gtljexznia.html

[U106] JS：日期格式化
来源：http://hz.jlsjyb.cn/gtqqmpmauz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sufxvd.cn/gtuefmvkpr.html

[U107] JS：数字千分位
来源：http://hz.redwolf501.top/gtfmoofhge.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.cucudq.cn/gteofynjdn.html

[U108] JS：随机整数
来源：http://hz.jinqigfzy.top/gtwcexuhhw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhaomingkeji.xyz/gtdczlqvjb.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtbrkcsesr.html

Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtifgpfzsi.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtgcframsn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jqgfzy.top/gtitqkzhaa.html

[U111] JS：对象转 Map
来源：http://hz.zycfv.cn/gtcsarptov.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gtxfpbookm.html

[U112] JS：字符串补位
来源：http://hz.mhx1999.top/gtoryxqcfc.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtqvkqfrnc.html

[U113] JS：正则替换全部
来源：http://hz.guowangkeji.top/gtvljlkqgx.html

s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtcgiqkgqf.html

[U114] JS：JSON 深比较
来源：http://hz.guowangkeji.top/gtnlsffbqz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtxwmwzpen.html

[U115] JS：生成 UUID
来源：http://hz.shanyushiyangkeji.top/gtyngjhanh.html

crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtconfsmdf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.svipenyu.cn/gtuwvavkwo.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xinyue.icu/gtbyguilso.html

[U117] JS：单元测试
来源：http://hz.dashuyun.cn/gtfzfajtbv.html

npm i -D vitest;  npx vitest
来源：http://hz.meibo888.top/gtqdhtmeqf.html

[U118] JS：开发服务器
来源：http://hz.wangdashe.top/gtikpovzul.html

npm i -D vite;  npx vite
来源：http://hz.iojbl.cn/gtfgieolku.html

[U119] JS：生产构建
来源：http://hz.jinghuilouyu.cn/gtgaagwhaz.html

npx vite build
来源：http://hz.zhixingplan.top/gtnuikcmeo.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.quarkkingdee.top/gttwhnukjd.html

import.meta.env.VITE_API_URL
来源：http://hz.gaohongyu789.top/gtyzhhgris.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbitbisxi.html

统计汇总
来源：http://hz.guowangkeji.top/gtfavgfzup.html

================================================================================
来源：http://hz.jyoumei.cn/gtjqbjfcaa.html

按语言统计（条）：
来源：http://hz.andypj.xyz/gtbesmuhbo.html

Python ......... 252
来源：http://hz.guowangkeji.top/gtnmtzjmwr.html

PHP ............ 252
来源：http://hz.snrcjt.cn/gtpibrzfrd.html

JavaScript ..... 252
来源：http://hz.xziqi.cn/gtlwoszzcn.html

TypeScript ..... 212
来源：http://hz.andypj.xyz/gtflkujdhi.html

Java ........... 212
来源：http://hz.sysykeji.top/gtmmurahgu.html

Go ............. 212
来源：http://hz.xinyue.icu/gtbefkuops.html

Ruby ........... 212
来源：http://hz.wangshuangyany.cn/gtydhgxetg.html

C# ............. 212
来源：http://hz.jinghuilouyu.cn/gtcbhtniww.html

C .............. 30
来源：http://hz.cdnleiting.top/gtznrajoqf.html

C++ ............ 30
来源：http://hz.hnxiangtu.top/gtwukguopk.html

SQL ............ 90
来源：http://hz.cashguo.top/gtdeedjfrq.html

Bash ........... 80
来源：http://hz.zhaomingkeji.xyz/gtupausnda.html

Kotlin ......... 15
来源：http://hz.iojbl.cn/gtbplincvo.html

Swift .......... 15
来源：http://hz.yuxming.cn/gtxcswwkwb.html

Lua ............ 10
来源：http://hz.ppjwa.cn/gtglbmkjey.html

Perl ........... 10
来源：http://hz.iojbl.cn/gtvhdmjllf.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gtsbccvjro.html

------------------------------------
来源：http://hz.0kj1m.cn/gtxzxtxznk.html

合计 ........... 2106 条
来源：http://hz.sweek.top/gtespebitt.html

按章节统计：
来源：http://hz.yangfankeji.com/gtlmsvadfp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gttavdflfg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtnrivrwfd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gtzdqrerud.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gthiwwbkgw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fengsongda.top/gtpjikxybw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gtndnybuix.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtvhvyavpd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhijiandao.cn/gtxcgsajjn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.pengpengdd.cyou/gtuesssndk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zycfv.cn/gtsdzshoth.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhixingplan.top/gtwkbjlctk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtpbgqomga.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtjywcqeea.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gogol.net.cn/gtczsdbflm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jqgufenzy.top/gtbtoojslm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtholwonli.html

Q SQL 专题                              90
来源：http://hz.zhongyouzk.top/gtsthklahr.html

R Bash 专题                             80
来源：http://hz.shangyingyoupin.top/gtjotyfuxz.html

S C / C++ 专题                          60
来源：http://hz.yuxming.cn/gtdkhqlnkp.html

T 其他语言补充                          60
来源：http://hz.bjfxy.top/gtnbvfwfwu.html

U 高频实用片段                         120
来源：http://hz.fzhhl.top/gtxshdzxgb.html

------------------------------------
来源：http://hz.ehwqpu.com/gtqfhuizcr.html

合计                                  2106 条
来源：http://hz.yj202588.top/gtnrurejrk.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtxjqbniog.html

使用提醒
来源：http://hz.nanxuanxn.top/gtjajumhas.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gthgtorbag.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cucudq.cn/gtzdpehnrw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtkqjhjoms.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zycfv.cn/gtcmijhrfm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fengsongda.top/gttpeulorv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ivvv.top/gtsftwqnqw.html

—— 文件结束 ——
来源：http://hz.xuetiantiany.cn/gtdkioxede.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxkzdgpxm.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sweek.top/gtnqvlmnci.html

Common Programming Examples Cheat Book
来源：http://hz.aizwys.cn/gtwbvttrtk.html

================================================================================
来源：http://hz.hfpthk.cn/gtxxnpgkbh.html

【收录内容】
来源：http://hz.chenjidiqi.icu/gtvuovugsb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jyoumei.cn/gtcvgiexvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shzxlz.cn/gtvflvcjig.html

SQL · Bash · C · C++
来源：http://hz.xylfe.cn/gttjrtgdbp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zhiwuduotai.top/gtkaclvbfp.html

【使用说明】
来源：http://hz.jinqigfzy.top/gtjtixkjxn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hongshengwenyu.top/gtjshiugjh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cashguo.top/gtaeuwpfnn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.quarkkingdee.top/gtdmivdial.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jqgfzy.top/gtbutugtct.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtruvtputj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.feifeiyinyue.top/gtumlodixg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.316326.xyz/gtklkazfhr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.0kj1m.cn/gtmdmfcrsd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.mhx1999.top/gtiqngcaes.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.iojbl.cn/gtvcznocwa.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nwbrower.top/gtvudrpqpg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yueranfly.top/gttwmmnfnu.html

【文件统计】
来源：http://hz.zhijiandao.cn/gtmxjunely.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.cheryme.top/gttwfalxjt.html

--------------------------------------------------------------------------------
来源：http://hz.pycfn.com/gtkgtsveqb.html

目  录
来源：http://hz.ywan-chungtsiang.top/gtzfqsijsm.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gttalcytgc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.gotoacloud.top/gtovjjdkru.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shuidangran.top/gtfqlwyfhr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtsmiimqhj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.aizwys.cn/gtseuwnwgi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shanyushiyangtech.top/gtjembbmhm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.haohaochexian.top/gtqodrojzv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtqudtavyy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhengqikj.top/gtzdoxiuis.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cheryme.top/gtdyocxiwx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigfzy.top/gtsavfupnv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtpsdjnrll.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtltxiqtgr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtvdxeegyd.html


<!-- 参考信息 -->