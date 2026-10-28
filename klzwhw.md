代发 wailian999

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtozfhpwoq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.iojbl.cn/gtwuhntasr.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gtsasgupcx.html

pat = re.compile(r"\d+")
来源：http://hz.sysykeji.top/gtpdcsphob.html

[U19] Py：正则替换带回调
来源：http://hz.gzhubu.top/gtkkurbfea.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtktpzavyi.html

[U20] Py：缓存函数结果
来源：http://hz.snrcjt.cn/gtbvsummub.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenzaomai.com/gtjrfxunas.html

[U21] Py：自定义上下文管理器
来源：http://hz.shangyingyoupin.top/gtfywlumai.html

@contextlib.contextmanager
来源：http://hz.mhx1999.top/gtyzgcgexb.html

[U22] Py：矩阵转置
来源：http://hz.havefunace.top/gtwspvzhus.html

list(zip(*m))
来源：http://hz.hnqzz.top/gtajjgmvny.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtwuuzijwp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtjyqmmekx.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gttzvckzed.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtcyeseygz.html

[U25] Py：CSV 按字典读
来源：http://hz.jlsjyb.cn/gttrypncym.html

csv.DictReader(f)
来源：http://hz.yongpay.top/gtogcumnuc.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gtsqjltqjc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnqzz.top/gtfebjcjwi.html

[U27] Py：异步 HTTP
来源：http://hz.xuanzx.com/gtbnmplpod.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.meibo888.top/gtzmaozobg.html

[U28] Py：类型别名
来源：http://hz.52xcode.cn/gtkneaeztr.html

UserId = int
来源：http://hz.9152youxi.cn/gtguigkdns.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtefosyfoe.html

@property 与 @x.setter 配合
来源：http://hz.shangyingyoupin.top/gtcqdzirmk.html

[U30] Py：数据类
来源：http://hz.havefunace.top/gtzlxuovhw.html

@dataclass(slots=True)
来源：http://hz.wangshuangyany.cn/gtojmuwzbg.html

[U31] Py：单测
来源：http://hz.quarkkingdee.top/gtqoottezn.html

python -m pytest -q
来源：http://hz.zdqjudy.top/gtvbuxipdf.html

[U32] Py：代码格式化
来源：http://hz.aizwys.cn/gtdwpatnfl.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtsafmhumb.html

[U33] Py：打包发布
来源：http://hz.sweek.top/gttetvjyix.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.0kj1m.cn/gtlkrjydsb.html

[U34] Py：判断编码
来源：http://hz.zhongyouzk.top/gtrufzkhdd.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gtgqshmpsh.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gtvvkyqgqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gtepofzwvo.html

[U36] Py：定时任务
来源：http://hz.andypj.xyz/gtsszkivwe.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtfwknudtd.html

[U37] Py：读写 Excel
来源：http://hz.hywenlv.cn/gtceqqtvky.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigufen.top/gtjlnshwrp.html

[U38] Py：获取脚本所在目录
来源：http://hz.pycfn.com/gtsharojte.html

Path(__file__).resolve().parent
来源：http://hz.fzhhl.top/gtuffdmuyi.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtynolumnt.html

sys.stdout.isatty()
来源：http://hz.dashuyun.cn/gtxughpsjn.html

[U40] Py：打印到标准错误
来源：http://hz.cdnleiting.top/gttnnlrbwx.html

print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtjpbvsjey.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtacmlphwn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangdashe.top/gtrpvcqhdo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.daria6918.cn/gtsrjfdjxn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangtech.top/gtajqdvdpm.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtbkxdjhwk.html

namespace App\Http;
来源：http://hz.havefunace.top/gtymppddqd.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtafqvkdqh.html

declare(strict_types=1);
来源：http://hz.yanxiufei.cn/gtxhyffioj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shuidangran.top/gthpttxqdi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtoilevvqs.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gtflkrhkzr.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtggsbidvm.html

[U47] PHP：联合类型
来源：http://hz.pycfn.com/gtiyvpfygx.html

int|string $id
来源：http://hz.gaohongyu789.top/gtpvtvfdoj.html

[U48] PHP：纯枚举
来源：http://hz.havefunace.top/gtrvzqlixo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yuxming.cn/gtchdxtejv.html

[U49] PHP：只读属性
来源：http://hz.daxiang520.top/gtjrzjwzjd.html

public readonly string $name
来源：http://hz.hammf.cn/gtpuzdipzo.html

[U50] PHP：构造器属性提升
来源：http://hz.xuanzx.com/gtyjwytlgw.html

public function __construct(private int $id) {}
来源：http://hz.nanxinkj.top/gtpkoinisp.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gtfqlheqsd.html

[$a, $b] = $arr;
来源：http://hz.chenlongwang.top/gtrjczwmzu.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtadzgekyj.html

$double = fn($x) => $x * 2;
来源：http://hz.zdqjudy.top/gtawqksfkt.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258888.top/gtrdcvpzfo.html

$v = $a ?? $b ?? "default";
来源：http://hz.dianchejie.cn/gtwpavyvmg.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtjtvjgeal.html

$obj?->method()
来源：http://hz.yangfankeji.com/gtcxculego.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtznxgwfvg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gtnlaurulh.html

[U56] PHP：命名参数
来源：http://hz.xylfe.cn/gtjhxlidjd.html

f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtvumvuqwr.html

[U57] PHP：字符串插值
来源：http://hz.daxiang520.top/gtozlcptcc.html

"值: {$a}"
来源：http://hz.yj202588.top/gtyvxyqbcp.html

[U58] PHP：数组三件套
来源：http://hz.52xcode.cn/gtzafpmrmw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258888.top/gtuqpxtqpu.html

[U59] PHP：自定义排序
来源：http://hz.yvedp.cn/gtjyhdffdj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtablrbxyq.html

[U60] PHP：JSON 编解码
来源：http://hz.xuanzx.com/gtwwvhakjo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xziqi.cn/gtptckojku.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtzzywrnih.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtstnnqcbt.html

[U62] PHP：日期对象
来源：http://hz.hammf.cn/gtgvjotahj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yongpay.top/gtjfvqwnnb.html

[U63] PHP：文件读写
来源：http://hz.jqgufenzy.top/gtufginbnd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.havefunace.top/gtpdtqnvwc.html

[U64] PHP：目录遍历
来源：http://hz.jlsjyb.cn/gtldqhyaeh.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.wangshuangyany.cn/gtyxegpkdr.html

[U65] PHP：会话
来源：http://hz.yonumen.top/gtfdpaginq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhengqikj.top/gtlgcytsbq.html

[U66] PHP：设置 Cookie
来源：http://hz.shzxlz.cn/gtrtspzadm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhoulong.xyz/gtmpmmkgex.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtxpneqlwn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.bjfxy.top/gtuudmfbit.html

[U68] PHP：PDO 连接
来源：http://hz.fengsongda.top/gtuczdhnxb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuanzx.com/gtjmtojslz.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtxgckygjq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ppjwa.cn/gtddrslubm.html

[U70] PHP：PDO 事务
来源：http://hz.cdnleiting.top/gtjqgtewtv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.wangdashe.top/gtxfaypslk.html

[U71] PHP：抛出异常
来源：http://hz.dashuyun.cn/gtixdkkmxf.html

throw new RuntimeException("失败", 500);
来源：http://hz.wangshuangyany.cn/gthdfjupyu.html

[U72] PHP：写错误日志
来源：http://hz.xuanzx.com/gtuawwspcg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hnxiangtu.top/gtmtxivleb.html

[U73] PHP：读取 ini 配置
来源：http://hz.andypj.xyz/gtnnxdoqpv.html

parse_ini_file("config.ini", true)
来源：http://hz.nwbrower.top/gtraqrkuac.html

[U74] PHP：读取环境变量
来源：http://hz.yj20258.top/gtoojulocd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jlsjyb.cn/gtekibbqcy.html

[U75] PHP：依赖注入
来源：http://hz.yvedp.cn/gtsjflrnht.html

composer require psr/container
来源：http://hz.ydzc1.top/gtpbgbkoix.html

[U76] PHP：简单路由
来源：http://hz.c1oappe.top/gtrydywcvn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.vqdsnc.cn/gtlgoxpgdu.html

[U77] PHP：模板渲染
来源：http://hz.dashuyun.cn/gtrnobmxbt.html

composer require twig/twig
来源：http://hz.gotoacloud.top/gtozfpouyn.html

[U78] PHP：单元测试
来源：http://hz.svipenyu.cn/gtasslnmnr.html

composer require --dev phpunit/phpunit
来源：http://hz.ydzc1.top/gtfpnazaea.html

[U79] PHP：静态分析
来源：http://hz.ybcxt.top/gtsrdiyxwp.html

composer require --dev phpstan/phpstan
来源：http://hz.cdnleiting.top/gtujassywu.html

[U80] PHP：代码规范修复
来源：http://hz.yuxming.cn/gtrgmrbhgw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hammf.cn/gtdqimcigw.html

[U81] JS：初始化项目
来源：http://hz.jinyuanbaomall.cn/gtvukjhkgf.html

npm init -y;  npm i express
来源：http://hz.yongpay.top/gtwzvsyyvo.html

[U82] JS：package.json 脚本
来源：http://hz.gotoacloud.top/gtlutrdplf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtszdmrxlc.html

[U83] JS：ES Module 导入导出
来源：http://hz.ehwqpu.com/gtkytaajvp.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhongyouzk.top/gtlicilurv.html

[U84] JS：CommonJS 写法
来源：http://hz.daxiang520.top/gtceeqfwxw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.haohaochexian.top/gtrhwwdymx.html

[U85] JS：可选链
来源：http://hz.zhijiandao.cn/gtrooadhbh.html

a?.b?.c
来源：http://hz.ydjk.org.cn/gtextuxhep.html

[U86] JS：空值合并
来源：http://hz.hnxiangtu.top/gtssazeijb.html

a ?? b
来源：http://hz.andypj.xyz/gtpvivchhe.html

[U87] JS：解构默认值
来源：http://hz.quarkkingdee.top/gtxkrxioaa.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yvedp.cn/gtcczchbfx.html

[U88] JS：对象展开合并
来源：http://hz.c1oappe.top/gtjpafheyf.html

{ ...a, ...b }
来源：http://hz.shzxlz.cn/gtffbhcryj.html

[U89] JS：数组去重
来源：http://hz.jinqigufen.top/gtiusoaurq.html

[...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtwgoeknlv.html

[U90] JS：数字数组排序
来源：http://hz.gotoacloud.top/gtouaznqav.html

[...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtbnhdfgzy.html

[U91] JS：对象键值遍历
来源：http://hz.nanxinkj.top/gttwjpnczn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.guowangkeji.top/gtwsosuivg.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gtldwlekqm.html

structuredClone(obj)
来源：http://hz.dashuyun.cn/gttlhttkqw.html

[U93] JS：模板字符串
来源：http://hz.hongshengwenyu.top/gtgzrcvdmz.html

`共 ${n} 条`
来源：http://hz.birdmap.top/gtkneaqjpt.html

[U94] JS：箭头函数
来源：http://hz.daxiang520.top/gtzcdvufkd.html

const double = x => x * 2;
来源：http://hz.sufxvd.cn/gtfihgkcam.html

[U95] JS：Promise 包装
来源：http://hz.yangfankeji.com/gtldkcgoip.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtmiuuvxgw.html

[U96] JS：async/await 与异常
来源：http://hz.gzhubu.top/gtdklzajtf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtraryskrm.html

[U97] JS：并发请求
来源：http://hz.iojbl.cn/gttnuephmh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtgvltbgmm.html

[U98] JS：fetch 带 JSON
来源：http://hz.jyoumei.cn/gtlrqoszmc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.wangdashe.top/gtuptifacf.html

[U99] JS：事件监听
来源：http://hz.hnxiangtu.top/gtyukclxzx.html

el.addEventListener("click", e => {})
来源：http://hz.yueranfly.top/gtvpvfgdnr.html

[U100] JS：DOM 查询
来源：http://hz.andypj.xyz/gticfzjllg.html

document.querySelector(".item")
来源：http://hz.mhx1999.top/gtmzfdygnc.html

[U101] JS：classList 操作
来源：http://hz.shzxlz.cn/gteaekykcv.html

el.classList.toggle("active")
来源：http://hz.haohaochexian.top/gtmqohgrjo.html

[U102] JS：本地存储
来源：http://hz.kuanghao11.cn/gtzglhpgdq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cqqwz.cn/gtsurijztg.html

[U103] JS：定时器
来源：http://hz.nanxinkj.top/gtonqqjyql.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gotoacloud.top/gtyruqiyyi.html

[U104] JS：防抖
来源：http://hz.gogol.net.cn/gtmvgjvrvk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hammf.cn/gtypyjhklx.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtktzuzlwt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.fzhhl.top/gtgpvopdnp.html

[U106] JS：日期格式化
来源：http://hz.jianghu66.top/gtrdanbwzd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sweek.top/gtejxyltzb.html

[U107] JS：数字千分位
来源：http://hz.52xcode.cn/gtegtgwrmj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ehwqpu.com/gtakvyhbsd.html

[U108] JS：随机整数
来源：http://hz.kuanghao11.cn/gtzgkccwad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.haohaochexian.top/gtwcsimbzh.html

[U109] JS：数组分组
来源：http://hz.ywan-chungtsiang.top/gtweaimdgb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtsjhahewl.html

[U110] JS：数组分块
来源：http://hz.chenjidiqi.icu/gtkohokdiu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.snrcjt.cn/gtzhhczfad.html

[U111] JS：对象转 Map
来源：http://hz.andypj.xyz/gtfrcsymuj.html

new Map(Object.entries(obj))
来源：http://hz.jyoumei.cn/gtartjtnwt.html

[U112] JS：字符串补位
来源：http://hz.wangshuangyany.cn/gttdqaclws.html

"7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtqprvhrsb.html

[U113] JS：正则替换全部
来源：http://hz.gogol.net.cn/gtluixezzw.html

s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtdkrlguth.html

[U114] JS：JSON 深比较
来源：http://hz.feifeiyinyue.top/gtgsvzqszp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtkxgmbgvn.html

[U115] JS：生成 UUID
来源：http://hz.jinghuilouyu.cn/gtijwqkkkl.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtmoywcvvz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxuanxn.top/gtfluqtmxc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.vqdsnc.cn/gteqhqyvhm.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangkeji.top/gtvamjsmmo.html

npm i -D vitest;  npx vitest
来源：http://hz.tian-w.cn/gtpgswrzhn.html

[U118] JS：开发服务器
来源：http://hz.tanke756.top/gtwpwicjwx.html

npm i -D vite;  npx vite
来源：http://hz.snrcjt.cn/gtykotuqsj.html

[U119] JS：生产构建
来源：http://hz.quarkkingdee.top/gtbqkdbgvt.html

npx vite build
来源：http://hz.yvedp.cn/gtadcvljan.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.andypj.xyz/gticvcoecm.html

import.meta.env.VITE_API_URL
来源：http://hz.ppjwa.cn/gtfinwwthr.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvfoxiwjx.html

统计汇总
来源：http://hz.bjfxy.top/gtvjkdjzji.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzkfsnaqe.html

按语言统计（条）：
来源：http://hz.xziqi.cn/gtinjyyawe.html

Python ......... 252
来源：http://hz.zhongyouzk.top/gtydatsczf.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gtnmpintjs.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gtmdmudhfg.html

TypeScript ..... 212
来源：http://hz.zhoulong.xyz/gtcgglsbnx.html

Java ........... 212
来源：http://hz.snrcjt.cn/gtipdxlxlv.html

Go ............. 212
来源：http://hz.vqdsnc.cn/gtdkahaaei.html

Ruby ........... 212
来源：http://hz.cqqwz.cn/gtdqbxoyof.html

C# ............. 212
来源：http://hz.yvedp.cn/gttfstgjzw.html

C .............. 30
来源：http://hz.chenjidiqi.icu/gtsmlhmhzt.html

C++ ............ 30
来源：http://hz.jinghuilouyu.cn/gtuockizhg.html

SQL ............ 90
来源：http://hz.yj20258.top/gtsexouxfc.html

Bash ........... 80
来源：http://hz.gaohongyu789.top/gtlbwwzqog.html

Kotlin ......... 15
来源：http://hz.ppjwa.cn/gtuvewlhqd.html

Swift .......... 15
来源：http://hz.mhx1999.top/gtfdbaavao.html

Lua ............ 10
来源：http://hz.zycfv.cn/gtcibotzes.html

Perl ........... 10
来源：http://hz.ywan-chungtsiang.top/gtckrzlscg.html

Scala .......... 10
来源：http://hz.zdqjudy.top/gtjjkibnhd.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gtpqenzgmz.html

合计 ........... 2106 条
来源：http://hz.hammf.cn/gtvnlgxray.html

按章节统计：
来源：http://hz.yonumen.top/gtvhtxrlbz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yongpay.top/gtsdvrmwfy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jlsjyb.cn/gtruswfyhy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtyqdxwetl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtosbbvgvy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtrgtttjrd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtrhulcjpm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtkzuiorhg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtdkoiklih.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtonyxmcoy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.sysykeji.top/gtftuswsuq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gttvuptlah.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtythybvfc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtesioiqve.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtqwiqxphd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenlongwang.top/gtxjgcfxlp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ppjwa.cn/gtcqkwiwyh.html

Q SQL 专题                              90
来源：http://hz.316326.xyz/gtxxdbxdig.html

R Bash 专题                             80
来源：http://hz.fzhhl.top/gtkghtneeh.html

S C / C++ 专题                          60
来源：http://hz.52xcode.cn/gtxstiyyrh.html

T 其他语言补充                          60
来源：http://hz.c1oappe.top/gtdlibpztb.html

U 高频实用片段                         120
来源：http://hz.jinghuilouyu.cn/gtvabpxmjk.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtsvtmptdm.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtkopbboef.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtpvadrxgu.html

使用提醒
来源：http://hz.cdnleiting.top/gtsxflkzyn.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtpxjujjva.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.mhx1999.top/gtofupagds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yanxiufei.cn/gtabifqern.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cdnleiting.top/gtkarbsaud.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zhengqikj.top/gtricpccra.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.52xcode.cn/gttokmniga.html

—— 文件结束 ——
来源：http://hz.andypj.xyz/gtuvizciit.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbgfxvccw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.andypj.xyz/gtdsqarepj.html

Common Programming Examples Cheat Book
来源：http://hz.bjfxy.top/gtadkvcncc.html

================================================================================
来源：http://hz.nwbrower.top/gtpfwdiuce.html

【收录内容】
来源：http://hz.zycfv.cn/gtsyzyfbnh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.shzxlz.cn/gtbysxksmn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydzc1.top/gtypgxqpuz.html

SQL · Bash · C · C++
来源：http://hz.ydzc1.top/gtlluoulil.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.svipenyu.cn/gtckniztkw.html

【使用说明】
来源：http://hz.cqqwz.cn/gtolgcykpe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.kuanghao11.cn/gtdkzjlqwb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ehwqpu.com/gtazxfbyof.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xziqi.cn/gtplenqszx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xinyue.icu/gtymmpwypr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtsrgvjqvg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.guowangkeji.top/gthdfhsovj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhengqikj.top/gtffrwvbjj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hammf.cn/gtugvmckjg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ydzc1.top/gtzxinjhwa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhaomingkeji.xyz/gtugdjghyn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.shanyushiyangtech.top/gtmxuqwqrx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nwbrower.top/gthetguqqz.html

【文件统计】
来源：http://hz.xziqi.cn/gtuvoeunis.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxuanxn.top/gtfqwcdomp.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtehhzkwma.html

目  录
来源：http://hz.jinqigfzy.top/gttljoaurl.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtmwsxivag.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtrgihweey.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtiwdiiyns.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gtditxgbzu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yuxming.cn/gtbzeloegt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.yonumen.top/gtajjcccuu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtttgsztcp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.pycfn.com/gtqbytkxya.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtjvuvjrfo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtgwcyqtnl.html


<!-- 参考信息 -->