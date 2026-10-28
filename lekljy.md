代发 wailian999

[U19] Py：正则替换带回调
来源：http://hz.zhaomingkeji.xyz/gtomsqkseq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinghuilouyu.cn/gtdtxkqyvj.html

[U20] Py：缓存函数结果
来源：http://hz.ehwqpu.com/gtlahcuxmd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtavlagbcq.html

[U21] Py：自定义上下文管理器
来源：http://hz.mhx1999.top/gtonwqnxye.html

@contextlib.contextmanager
来源：http://hz.wangdashe.top/gtpxkobkxi.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtmhrokixz.html

list(zip(*m))
来源：http://hz.zhixingplan.top/gtkpkeyybs.html

[U23] Py：分块读取大文件
来源：http://hz.tian-w.cn/gtmdgobdcg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangkeji.top/gtqiqvvzzc.html

[U24] Py：路径操作
来源：http://hz.daxiang520.top/gtytlhycex.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guannengcc.top/gtxefwskyx.html

[U25] Py：CSV 按字典读
来源：http://hz.pengpengdd.cyou/gtlvoxmfpd.html

csv.DictReader(f)
来源：http://hz.daria6918.cn/gtjtpwhfxv.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtqbzupqdc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xylfe.cn/gtnexkjxcw.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtvixpyyei.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhijiandao.cn/gtgvssgfsz.html

[U28] Py：类型别名
来源：http://hz.xylfe.cn/gtdsopdacj.html

UserId = int
来源：http://hz.nanxuanxn.top/gtmhtudcsv.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtjgomcksz.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtnzpgglme.html

[U30] Py：数据类
来源：http://hz.hnqzz.top/gtymtccqdp.html

@dataclass(slots=True)
来源：http://hz.gogol.net.cn/gtqaqwqkls.html

[U31] Py：单测
来源：http://hz.xylfe.cn/gtotqpyiwj.html

python -m pytest -q
来源：http://hz.xuetiantiany.cn/gtgrdxivig.html

[U32] Py：代码格式化
来源：http://hz.52xcode.cn/gtljpbvahk.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtjkkxexbi.html

[U33] Py：打包发布
来源：http://hz.jlsjyb.cn/gtqtlifcdf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuxming.cn/gtipdktinj.html

[U34] Py：判断编码
来源：http://hz.cqqwz.cn/gtbviqhxkk.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtvfdfbczq.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gtwnkxgrpq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yj20258.top/gtrakenyip.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtbkrgylkp.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenlongwang.top/gtxcqnrche.html

[U37] Py：读写 Excel
来源：http://hz.zhongyouzk.top/gtvccbqjra.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zycfv.cn/gtkcxscxsl.html

[U38] Py：获取脚本所在目录
来源：http://hz.birdmap.top/gtydbhjdph.html

Path(__file__).resolve().parent
来源：http://hz.pengpengdd.cyou/gtpvgtltgz.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtiixmznfx.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gttorisilq.html

[U40] Py：打印到标准错误
来源：http://hz.ydzc1.top/gtgfvswuhj.html

print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtzotjpnfz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.haohaochexian.top/gtmgqwycjl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.pengpengdd.cyou/gtzlbrynqi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ydzc1.top/gtbeiflgno.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ehwqpu.com/gtywrbplse.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtxaxgrgnc.html

namespace App\Http;
来源：http://hz.nanxuanxn.top/gtjytenbgj.html

[U44] PHP：开启严格类型
来源：http://hz.fengsongda.top/gtygsgeotj.html

declare(strict_types=1);
来源：http://hz.jiagoushi.top/gthqsgxeks.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtmbomzfpd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtqwlbnpjx.html

[U46] PHP：可空类型
来源：http://hz.svipenyu.cn/gtgphwthbh.html

?string $name = null
来源：http://hz.ydzc1.top/gtfplnadsd.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangtech.top/gtdwtilroa.html

int|string $id
来源：http://hz.jianghu66.top/gtdgkxpzqy.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtrgiwnwjs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258.top/gtuhomzwwd.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtcqbfibqs.html

public readonly string $name
来源：http://hz.birdmap.top/gtnsgranzu.html

[U50] PHP：构造器属性提升
来源：http://hz.xziqi.cn/gtmvjtkgkb.html

public function __construct(private int $id) {}
来源：http://hz.jianghu66.top/gtcpegucxo.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gtlpdkugsk.html

[$a, $b] = $arr;
来源：http://hz.316326.xyz/gtfmjmzyuu.html

[U52] PHP：箭头函数
来源：http://hz.hongshengwenyu.top/gthtuszlwq.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgfzy.top/gthcbncyiq.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtpvljlkdx.html

$v = $a ?? $b ?? "default";
来源：http://hz.vqdsnc.cn/gtyudqnevc.html

[U54] PHP：空安全调用
来源：http://hz.hongshengwenyu.top/gtloqbunvo.html

$obj?->method()
来源：http://hz.jqgfzy.top/gtrlqjbrbf.html

[U55] PHP：match 表达式
来源：http://hz.guannengcc.top/gtspmvgqdm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gotoacloud.top/gtjnqsueep.html

[U56] PHP：命名参数
来源：http://hz.yvedp.cn/gtjxawxbaq.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtctkenrzi.html

[U57] PHP：字符串插值
来源：http://hz.xziqi.cn/gtosquzpcc.html

"值: {$a}"
来源：http://hz.jinyuanbaomall.cn/gtwueatlbf.html

[U58] PHP：数组三件套
来源：http://hz.ivvv.top/gthzozqukx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gttnmblcag.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtpkeivnkp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.svipenyu.cn/gttqsvbqro.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgfzy.top/gtzsdztzzi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenzaomai.com/gtxribbymt.html

[U61] PHP：正则
来源：http://hz.guannengcc.top/gtgxixmwnr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtcomsnivw.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gtogsbhxxs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhengqikj.top/gtbghmzymw.html

[U63] PHP：文件读写
来源：http://hz.zhijiandao.cn/gtnbfafgfz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtdjvtgtfe.html

[U64] PHP：目录遍历
来源：http://hz.shanyushiyangtech.top/gtiongevsb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtomrygrdf.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gtxghudhjx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gogol.net.cn/gtgyetcedf.html

[U66] PHP：设置 Cookie
来源：http://hz.ivvv.top/gtryibamfi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xingfuxueyuan.xyz/gtnjrpuqlq.html

[U67] PHP：处理文件上传
来源：http://hz.316326.xyz/gtyljqlteh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.pengpengdd.cyou/gtsyndeoej.html

[U68] PHP：PDO 连接
来源：http://hz.xylfe.cn/gtbrsfalnr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zdqjudy.top/gtmyrnbkyn.html

[U69] PHP：PDO 预处理
来源：http://hz.feifeiyinyue.top/gtmsvygzyf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.svipenyu.cn/gtlyyghwpd.html

[U70] PHP：PDO 事务
来源：http://hz.shanyushiyangkeji.top/gtiqxdorqy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yvedp.cn/gtjkorlgil.html

[U71] PHP：抛出异常
来源：http://hz.jianghu66.top/gtqipsoqet.html

throw new RuntimeException("失败", 500);
来源：http://hz.zdqjudy.top/gtgbmgnupg.html

[U72] PHP：写错误日志
来源：http://hz.sweek.top/gtvsgvvapl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.svipenyu.cn/gtxkppknmz.html

[U73] PHP：读取 ini 配置
来源：http://hz.yangfankeji.com/gtitxcrzfq.html

parse_ini_file("config.ini", true)
来源：http://hz.yongpay.top/gtcwvwaicb.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtlywbzvwb.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258888.top/gtqrgdpqht.html

[U75] PHP：依赖注入
来源：http://hz.gogol.net.cn/gtqqmrdwjk.html

composer require psr/container
来源：http://hz.yangfankeji.com/gtfzkxcpzu.html

[U76] PHP：简单路由
来源：http://hz.jqgfzy.top/gtuhwzwigc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xuanzx.com/gtlkusqybe.html

[U77] PHP：模板渲染
来源：http://hz.jinqigfzy.top/gtdkbjexfw.html

composer require twig/twig
来源：http://hz.aizwys.cn/gttbrbaggy.html

[U78] PHP：单元测试
来源：http://hz.hnxiangtu.top/gtmhelbxif.html

composer require --dev phpunit/phpunit
来源：http://hz.yanxiufei.cn/gtudiadkmn.html

[U79] PHP：静态分析
来源：http://hz.shanyushiyangkeji.top/gtblsatchs.html

composer require --dev phpstan/phpstan
来源：http://hz.jinghuilouyu.cn/gttuiwufpb.html

[U80] PHP：代码规范修复
来源：http://hz.cheryme.top/gtasbdfzei.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jinqigfzy.top/gtzxqvphys.html

[U81] JS：初始化项目
来源：http://hz.tian-w.cn/gtytdclbpo.html

npm init -y;  npm i express
来源：http://hz.cdnleiting.top/gtystqkqyz.html

[U82] JS：package.json 脚本
来源：http://hz.cdnleiting.top/gtvvrzkbjf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sufxvd.cn/gtxktwgwmx.html

[U83] JS：ES Module 导入导出
来源：http://hz.feifeiyinyue.top/gtwofzmajf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj20258888.top/gtquwvafgc.html

[U84] JS：CommonJS 写法
来源：http://hz.52xcode.cn/gtqgbubfir.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.feifeiyinyue.top/gtpszylyst.html

[U85] JS：可选链
来源：http://hz.aizwys.cn/gtvzwlbmsj.html

a?.b?.c
来源：http://hz.havefunace.top/gtzxqybqng.html

[U86] JS：空值合并
来源：http://hz.zhongyouzk.top/gtdvqtmsfu.html

a ?? b
来源：http://hz.shangyingyoupin.top/gtemodpumi.html

[U87] JS：解构默认值
来源：http://hz.mhx1999.top/gtiealidnm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sysykeji.top/gtplcnyvuf.html

[U88] JS：对象展开合并
来源：http://hz.svipenyu.cn/gtrndsfuzn.html

{ ...a, ...b }
来源：http://hz.tian-w.cn/gthwanpfln.html

[U89] JS：数组去重
来源：http://hz.havefunace.top/gtsrdszpai.html

[...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtognranen.html

[U90] JS：数字数组排序
来源：http://hz.yanxiufei.cn/gtzqyuggxv.html

[...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtrltfeksl.html

[U91] JS：对象键值遍历
来源：http://hz.yj20258888.top/gtxropvspj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhoulong.xyz/gtjcgdhqwl.html

[U92] JS：深拷贝
来源：http://hz.gogol.net.cn/gtccprndft.html

structuredClone(obj)
来源：http://hz.yueranfly.top/gtkeznvpsm.html

[U93] JS：模板字符串
来源：http://hz.shanyushiyangtech.top/gtncadnfxq.html

`共 ${n} 条`
来源：http://hz.vqdsnc.cn/gtuworoqyn.html

[U94] JS：箭头函数
来源：http://hz.hnxiangtu.top/gtuqrlzuzz.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtfqwtlwxz.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangkeji.top/gtdcuxbvvm.html

new Promise((resolve, reject) => {})
来源：http://hz.zycfv.cn/gtkktjefor.html

[U96] JS：async/await 与异常
来源：http://hz.zhoulong.xyz/gtzmfwckvf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtfdopfdyw.html

[U97] JS：并发请求
来源：http://hz.chenzaomai.com/gtexdgbwgj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtumidzvue.html

[U98] JS：fetch 带 JSON
来源：http://hz.guowangkeji.top/gtyhpacgiq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhongyouzk.top/gthueddplo.html

[U99] JS：事件监听
来源：http://hz.ydjk.org.cn/gtrajlydeq.html

el.addEventListener("click", e => {})
来源：http://hz.nanxuanxn.top/gtcoifidrt.html

[U100] JS：DOM 查询
来源：http://hz.dashuyun.cn/gtzrrxzgwd.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gtrunwbbvs.html

[U101] JS：classList 操作
来源：http://hz.jqgfzy.top/gttvvdzsia.html

el.classList.toggle("active")
来源：http://hz.mhx1999.top/gtcwuwvarf.html

[U102] JS：本地存储
来源：http://hz.aizwys.cn/gtmzgklajq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.haohaochexian.top/gtmaoemhjd.html

[U103] JS：定时器
来源：http://hz.svipenyu.cn/gtykrvubxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.pycfn.com/gtrvkugaoj.html

[U104] JS：防抖
来源：http://hz.chenjidiqi.icu/gtctxhfsqi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtopkgynxp.html

[U105] JS：节流
来源：http://hz.ydzc1.top/gtnbnbnbpe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.bjfxy.top/gtzfyzbnwb.html

[U106] JS：日期格式化
来源：http://hz.cqqwz.cn/gtbvzrgifa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.daxiang520.top/gtwqnxqbno.html

[U107] JS：数字千分位
来源：http://hz.cucudq.cn/gtasmgacdc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.daxiang520.top/gtifxnbbwd.html

[U108] JS：随机整数
来源：http://hz.hnqzz.top/gtmdgbunqe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtszykgtqs.html

[U109] JS：数组分组
来源：http://hz.yj20258888.top/gtvcdxqcff.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtabflbmky.html

[U110] JS：数组分块
来源：http://hz.quarkkingdee.top/gtwdgqgnmo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.meibo888.top/gtuylncspd.html

[U111] JS：对象转 Map
来源：http://hz.ivvv.top/gtzbyrwdgi.html

new Map(Object.entries(obj))
来源：http://hz.ehwqpu.com/gtsjmxtpdy.html

[U112] JS：字符串补位
来源：http://hz.zdqjudy.top/gtfanobqca.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtldrdujjl.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtftykekaa.html

s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtlrrflxjy.html

[U114] JS：JSON 深比较
来源：http://hz.yueranfly.top/gtotdyvpts.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ivvv.top/gtxxtzdfvp.html

[U115] JS：生成 UUID
来源：http://hz.52xcode.cn/gttxmrfqqk.html

crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtvltqexrl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gthzsajlaf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258.top/gtrzzkalbi.html

[U117] JS：单元测试
来源：http://hz.jqgufenzy.top/gtffcaucvw.html

npm i -D vitest;  npx vitest
来源：http://hz.hywenlv.cn/gtzqbdseuv.html

[U118] JS：开发服务器
来源：http://hz.hammf.cn/gtswlrowyk.html

npm i -D vite;  npx vite
来源：http://hz.yangfankeji.com/gtryyijmtn.html

[U119] JS：生产构建
来源：http://hz.zhiwuduotai.top/gttjfnxngo.html

npx vite build
来源：http://hz.yvedp.cn/gthyuwqwkz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jinyuanbaomall.cn/gtrhhbilpt.html

import.meta.env.VITE_API_URL
来源：http://hz.pengpengdd.cyou/gtitmvezoi.html

================================================================================
来源：http://hz.tianlin.xyz/gtjrresrwe.html

统计汇总
来源：http://hz.ivvv.top/gtklswghtq.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtobwkvlrq.html

按语言统计（条）：
来源：http://hz.jinyuanbaomall.cn/gtnuuqxypr.html

Python ......... 252
来源：http://hz.tianlin.xyz/gtmutelfde.html

PHP ............ 252
来源：http://hz.shangyingyoupin.top/gtppramtln.html

JavaScript ..... 252
来源：http://hz.jinqigfzy.top/gtfavetevr.html

TypeScript ..... 212
来源：http://hz.kuanghao11.cn/gtkscuprma.html

Java ........... 212
来源：http://hz.xuanzx.com/gtjmkplxcv.html

Go ............. 212
来源：http://hz.yonumen.top/gtyusgizqj.html

Ruby ........... 212
来源：http://hz.c1oappe.top/gtkbrvxupn.html

C# ............. 212
来源：http://hz.pycfn.com/gtgjqnccoo.html

C .............. 30
来源：http://hz.jyoumei.cn/gtcluvvhdw.html

C++ ............ 30
来源：http://hz.ivvv.top/gtonwxrfpi.html

SQL ............ 90
来源：http://hz.yj202588.top/gtczocvfox.html

Bash ........... 80
来源：http://hz.nanxinkj.top/gtaexdkfog.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gttlttxjgo.html

Swift .......... 15
来源：http://hz.cucudq.cn/gtjfcxcfpi.html

Lua ............ 10
来源：http://hz.zhongyouzk.top/gtiabnenje.html

Perl ........... 10
来源：http://hz.yvedp.cn/gtuaxycsmi.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtunuhdsac.html

------------------------------------
来源：http://hz.chenzaomai.com/gtpgsswsxe.html

合计 ........... 2106 条
来源：http://hz.316326.xyz/gtzslpswyw.html

按章节统计：
来源：http://hz.pycfn.com/gtnoqkdbwg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.tianlin.xyz/gtyvuspylo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gthxrcasnb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gtceqmekhl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yongpay.top/gtulcmztmd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sxryk.cn/gtmrzioyjv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtozmxdibh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gtuolgmyki.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gthwugynyw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtvnvqnnni.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtrhcaeevk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtnbftsgsi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtxrkeojfo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gttiolldng.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtrnosdcav.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jiagoushi.top/gtkotoncdn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtftxoktdd.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangkeji.top/gttwffbpyl.html

R Bash 专题                             80
来源：http://hz.chenlongwang.top/gtpictqzyz.html

S C / C++ 专题                          60
来源：http://hz.jinghuilouyu.cn/gtqjhljhqu.html

T 其他语言补充                          60
来源：http://hz.vqdsnc.cn/gtgrvvaeuf.html

U 高频实用片段                         120
来源：http://hz.ybcxt.top/gtevswzykv.html

------------------------------------
来源：http://hz.hammf.cn/gtchcmzknu.html

合计                                  2106 条
来源：http://hz.wangdashe.top/gtcrpcfteq.html

--------------------------------------------------------------------------------
来源：http://hz.chenjidiqi.icu/gtpoqfpftc.html

使用提醒
来源：http://hz.shuidangran.top/gtxkcuenth.html

--------------------------------------------------------------------------------
来源：http://hz.shangyingyoupin.top/gtaebqaijj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinyuanbaomall.cn/gtlajayowr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fzhhl.top/gtvrthswjz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.316326.xyz/gtbhrrsigo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nwbrower.top/gtzcvzblif.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.haohaochexian.top/gtegoohltt.html

—— 文件结束 ——
来源：http://hz.haohaochexian.top/gtmbmdsezq.html

================================================================================
来源：http://hz.hfpthk.cn/gtmvxakoum.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinyuanbaomall.cn/gtfojypylt.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigfzy.top/gtpdgyqpna.html

================================================================================
来源：http://hz.cashguo.top/gtvkpwksly.html

【收录内容】
来源：http://hz.hfpthk.cn/gtiphhpdkg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shangyingyoupin.top/gtkjmidibx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhaomingkeji.xyz/gtnmhfrghv.html

SQL · Bash · C · C++
来源：http://hz.fengsongda.top/gtdvwjndoj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.fengsongda.top/gtlkgdimho.html

【使用说明】
来源：http://hz.cashguo.top/gtnsqgwclv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.aizwys.cn/gtujyuvssl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.dashuyun.cn/gtqlrmuttt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.guannengcc.top/gthhwzdiqf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yuxming.cn/gtccwbmtys.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.c1oappe.top/gtkrplhpft.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xylfe.cn/gtzrvqjfzw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenzaomai.com/gtvyfvvmbl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ydjk.org.cn/gtenoxdvmr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtykdammau.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.birdmap.top/gtlmvvhuyg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nwbrower.top/gtfottrkzh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jinghuilouyu.cn/gtcbebuzfi.html

【文件统计】
来源：http://hz.ydjk.org.cn/gtdtgjmhcw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.9152youxi.cn/gtwsfjoofu.html

--------------------------------------------------------------------------------
来源：http://hz.jiagoushi.top/gtgbuegctc.html

目  录
来源：http://hz.pycfn.com/gtwbpeixgs.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtkhwtyvik.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenzaomai.com/gtgdujkvzd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.chenzaomai.com/gtdsqbvomj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtezoaydaz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gthtktqixy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtqypzjjka.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.hnqzz.top/gttpknqzsl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yanxiufei.cn/gtxqbhcuxr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nwbrower.top/gtliqkqhvj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.smart0.xyz/gtoiwahxeu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.chenlongwang.top/gtmiicxfkd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtbkjbabdy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nanxinkj.top/gtyczeabou.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtlfhgkgwa.html


<!-- 参考信息 -->