代发 wailian999

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gtedsyahpu.html

deque(maxlen=10)
来源：http://hz.meibo888.top/gtztfcorbg.html

[U14] Py：分组收集到列表
来源：http://hz.nwbrower.top/gtqvulsvid.html

defaultdict(list)
来源：http://hz.xylfe.cn/gtoazidgfw.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtecfikczr.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gtzescfzpt.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtwxgfszmr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jiagoushi.top/gttvgfhetg.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtkizbtwum.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fzhhl.top/gttpcshbey.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtwclqwcvo.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gtanduqyus.html

[U19] Py：正则替换带回调
来源：http://hz.ehwqpu.com/gtrpdrgqiq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pengpengdd.cyou/gtlzsvszuz.html

[U20] Py：缓存函数结果
来源：http://hz.ydjk.org.cn/gtgyybtmhq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.316326.xyz/gtochubpyv.html

[U21] Py：自定义上下文管理器
来源：http://hz.daxiang520.top/gtzgzycmsb.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtagcjzvui.html

[U22] Py：矩阵转置
来源：http://hz.chenlongwang.top/gtgaalmsfi.html

list(zip(*m))
来源：http://hz.daria6918.cn/gtwabdolpu.html

[U23] Py：分块读取大文件
来源：http://hz.snrcjt.cn/gtygkgcqkh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtuqrmdbks.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtdwwfbgow.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtjixgjexr.html

[U25] Py：CSV 按字典读
来源：http://hz.ydjk.org.cn/gttmscoxsy.html

csv.DictReader(f)
来源：http://hz.nanxuanxn.top/gtzbnwynln.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtwywzlxxd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuxming.cn/gtqmomzkeb.html

[U27] Py：异步 HTTP
来源：http://hz.hfpthk.cn/gtdecalrxu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhongyouzk.top/gtgiylbogw.html

[U28] Py：类型别名
来源：http://hz.jlsjyb.cn/gtdqibshiw.html

UserId = int
来源：http://hz.vqdsnc.cn/gthawempid.html

[U29] Py：属性校验
来源：http://hz.pengpengdd.cyou/gtmqvqljfx.html

@property 与 @x.setter 配合
来源：http://hz.cdnleiting.top/gtzapbzesd.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtexyieivk.html

@dataclass(slots=True)
来源：http://hz.quarkkingdee.top/gtilnybfbp.html

[U31] Py：单测
来源：http://hz.nanxinkj.top/gtchxczhck.html

python -m pytest -q
来源：http://hz.ivvv.top/gtnrqsbfqr.html

[U32] Py：代码格式化
来源：http://hz.xinyue.icu/gtrvldzndf.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtqbavelyu.html

[U33] Py：打包发布
来源：http://hz.wangdashe.top/gtjqptjceu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenjidiqi.icu/gtarubdljv.html

[U34] Py：判断编码
来源：http://hz.haohaochexian.top/gtcwugtmns.html

chardet.detect(raw)
来源：http://hz.fzhhl.top/gtckbrvvjh.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gteaphjoyr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuanzx.com/gtdaofgfen.html

[U36] Py：定时任务
来源：http://hz.nwbrower.top/gtddyrjyhy.html

schedule.every(10).minutes.do(job)
来源：http://hz.pycfn.com/gtcjcdbfmi.html

[U37] Py：读写 Excel
来源：http://hz.zhongyouzk.top/gttobzofsq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yueranfly.top/gtkydxemiz.html

[U38] Py：获取脚本所在目录
来源：http://hz.yuanzhike.top/gtmyzxpojm.html

Path(__file__).resolve().parent
来源：http://hz.yangfankeji.com/gtdellgxqa.html

[U39] Py：判断是否在交互环境
来源：http://hz.smart0.xyz/gtzkwwkwnb.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtumbruwkw.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtwdcsoxdm.html

print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtpfiobdxh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenzaomai.com/gtkbvqmpec.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.svipenyu.cn/gtmjavcwtj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.svipenyu.cn/gtwctjjdbu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yangfankeji.com/gttqmnrwmy.html

[U43] PHP：声明命名空间
来源：http://hz.ehwqpu.com/gtylvmtgdf.html

namespace App\Http;
来源：http://hz.daria6918.cn/gtrrsfrtar.html

[U44] PHP：开启严格类型
来源：http://hz.jiagoushi.top/gtkjsaqgbl.html

declare(strict_types=1);
来源：http://hz.ybcxt.top/gtaszfhlxi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtsgmpqwfe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtajunjnkp.html

[U46] PHP：可空类型
来源：http://hz.hnxiangtu.top/gtdyjfgbwd.html

?string $name = null
来源：http://hz.ppjwa.cn/gtsuaxsesv.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gttjhaoeyd.html

int|string $id
来源：http://hz.sweek.top/gtrvzsqnfr.html

[U48] PHP：纯枚举
来源：http://hz.c1oappe.top/gtqchbvisr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258888.top/gtyrcriigl.html

[U49] PHP：只读属性
来源：http://hz.jiagoushi.top/gtafdtncbv.html

public readonly string $name
来源：http://hz.guannengcc.top/gtapuhteer.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtxjlirpbo.html

public function __construct(private int $id) {}
来源：http://hz.redwolf501.top/gtbcfmbasw.html

[U51] PHP：数组解构
来源：http://hz.havefunace.top/gtryeyxyih.html

[$a, $b] = $arr;
来源：http://hz.aibaodan.cn/gtmvaeanly.html

[U52] PHP：箭头函数
来源：http://hz.jianghu66.top/gtbjtotwhe.html

$double = fn($x) => $x * 2;
来源：http://hz.feifeiyinyue.top/gtgedgtawq.html

[U53] PHP：空合并运算符
来源：http://hz.ybcxt.top/gtpkrkwfhy.html

$v = $a ?? $b ?? "default";
来源：http://hz.pycfn.com/gtdeznhxgp.html

[U54] PHP：空安全调用
来源：http://hz.52xcode.cn/gtyontzlyd.html

$obj?->method()
来源：http://hz.snrcjt.cn/gtahagrbxn.html

[U55] PHP：match 表达式
来源：http://hz.ybcxt.top/gtyuafwdlc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtppeabipz.html

[U56] PHP：命名参数
来源：http://hz.cqqwz.cn/gtvzivlwtl.html

f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtrdniyrml.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtkvhgintj.html

"值: {$a}"
来源：http://hz.ppjwa.cn/gtpozryyjr.html

[U58] PHP：数组三件套
来源：http://hz.xziqi.cn/gtgkeygdut.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cheryme.top/gtexcswiiv.html

[U59] PHP：自定义排序
来源：http://hz.jinghuilouyu.cn/gtfbtaklrq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtpeuzpqov.html

[U60] PHP：JSON 编解码
来源：http://hz.yonumen.top/gtohokdpfi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zycfv.cn/gtwquosmlp.html

[U61] PHP：正则
来源：http://hz.gotoacloud.top/gtdrdjojpn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtiyauwwpl.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtylmuubwr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.feifeiyinyue.top/gteohxbaad.html

[U63] PHP：文件读写
来源：http://hz.ywan-chungtsiang.top/gtpivjbots.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigufen.top/gtmqhtlhfi.html

[U64] PHP：目录遍历
来源：http://hz.iojbl.cn/gtjpxhbrno.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtwhxeyina.html

[U65] PHP：会话
来源：http://hz.zycfv.cn/gtfqimlofd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj20258.top/gtypdkcxdc.html

[U66] PHP：设置 Cookie
来源：http://hz.yonumen.top/gtawwgihxm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.daxiang520.top/gtnoykcwmn.html

[U67] PHP：处理文件上传
来源：http://hz.ppjwa.cn/gtldxryfip.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hnqzz.top/gtubbuthvo.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gtzhiooedx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pengpengdd.cyou/gtshpqgxuu.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtfjvjioze.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.vqdsnc.cn/gtsysnaonh.html

[U70] PHP：PDO 事务
来源：http://hz.yuanzhike.top/gtgkyigbjo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtvvisvini.html

[U71] PHP：抛出异常
来源：http://hz.snrcjt.cn/gtdubrcaew.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj202588.top/gtfhjnuzxx.html

[U72] PHP：写错误日志
来源：http://hz.yj202588.top/gtsjyquaxy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.316326.xyz/gtraisdvit.html

[U73] PHP：读取 ini 配置
来源：http://hz.0kj1m.cn/gturcnboec.html

parse_ini_file("config.ini", true)
来源：http://hz.ywan-chungtsiang.top/gtdhmyvzim.html

[U74] PHP：读取环境变量
来源：http://hz.birdmap.top/gttycjbycy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gaohongyu789.top/gtdrjzpcln.html

[U75] PHP：依赖注入
来源：http://hz.jiagoushi.top/gtosautskk.html

composer require psr/container
来源：http://hz.xylfe.cn/gtrmijooon.html

[U76] PHP：简单路由
来源：http://hz.tian-w.cn/gtzmrgghls.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hnxiangtu.top/gtpigdgldz.html

[U77] PHP：模板渲染
来源：http://hz.nanxuanxn.top/gtqoweigbw.html

composer require twig/twig
来源：http://hz.svipenyu.cn/gtqfjpfmwe.html

[U78] PHP：单元测试
来源：http://hz.shuidangran.top/gttqsrjcgy.html

composer require --dev phpunit/phpunit
来源：http://hz.shangyingyoupin.top/gtluqstxja.html

[U79] PHP：静态分析
来源：http://hz.redwolf501.top/gtdswczcqo.html

composer require --dev phpstan/phpstan
来源：http://hz.yongpay.top/gtryhjuqtu.html

[U80] PHP：代码规范修复
来源：http://hz.meibo888.top/gtkgjwrxut.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhengqikj.top/gtbivuthbq.html

[U81] JS：初始化项目
来源：http://hz.sxryk.cn/gtbhswulbh.html

npm init -y;  npm i express
来源：http://hz.havefunace.top/gtvwnjficg.html

[U82] JS：package.json 脚本
来源：http://hz.gogol.net.cn/gtllvjdrag.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shuidangran.top/gtiizdpdsj.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtwzowvowt.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhixingplan.top/gtzlohehdp.html

[U84] JS：CommonJS 写法
来源：http://hz.sxryk.cn/gtfbjqjdft.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gtoucerkic.html

[U85] JS：可选链
来源：http://hz.ivvv.top/gtmswqxhqd.html

a?.b?.c
来源：http://hz.zhijiandao.cn/gtoqrttabi.html

[U86] JS：空值合并
来源：http://hz.vqdsnc.cn/gtuleoaeyf.html

a ?? b
来源：http://hz.birdmap.top/gtjwrnawlq.html

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtfqmsykon.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shanyushiyangtech.top/gtjpyhabvu.html

[U88] JS：对象展开合并
来源：http://hz.sxryk.cn/gtflbcwjyu.html

{ ...a, ...b }
来源：http://hz.andypj.xyz/gtkuanlmkw.html

[U89] JS：数组去重
来源：http://hz.sufxvd.cn/gtqgekvlbv.html

[...new Set(arr)]
来源：http://hz.dashuyun.cn/gtocqyisyg.html

[U90] JS：数字数组排序
来源：http://hz.guowangkeji.top/gtsdfxvnfe.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtnqwgoyca.html

[U91] JS：对象键值遍历
来源：http://hz.ybcxt.top/gtamxrrnjr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gaohongyu789.top/gtysfqsteb.html

[U92] JS：深拷贝
来源：http://hz.snrcjt.cn/gtboyhnlpg.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtxcuavgso.html

[U93] JS：模板字符串
来源：http://hz.zhixingplan.top/gtomcbeltw.html

`共 ${n} 条`
来源：http://hz.pengpengdd.cyou/gtezzfljgu.html

[U94] JS：箭头函数
来源：http://hz.52xcode.cn/gtpyeyitdk.html

const double = x => x * 2;
来源：http://hz.haohaochexian.top/gtkjuzqmjo.html

[U95] JS：Promise 包装
来源：http://hz.nanxuanxn.top/gttctdvpnb.html

new Promise((resolve, reject) => {})
来源：http://hz.chenzaomai.com/gtcudpcxqg.html

[U96] JS：async/await 与异常
来源：http://hz.zhixingplan.top/gtgryxdrba.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtciindald.html

[U97] JS：并发请求
来源：http://hz.andypj.xyz/gtjqhhqduf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtxesbwnpg.html

[U98] JS：fetch 带 JSON
来源：http://hz.316326.xyz/gtepnngzdd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yongpay.top/gtkuceedkc.html

[U99] JS：事件监听
来源：http://hz.ywan-chungtsiang.top/gtefgbhteq.html

el.addEventListener("click", e => {})
来源：http://hz.zycfv.cn/gtrqefjcnj.html

[U100] JS：DOM 查询
来源：http://hz.zdqjudy.top/gtmbkteuel.html

document.querySelector(".item")
来源：http://hz.yangfankeji.com/gtrwoqxuxy.html

[U101] JS：classList 操作
来源：http://hz.yonumen.top/gtgodhevjm.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangtech.top/gtpmfbqftg.html

[U102] JS：本地存储
来源：http://hz.yangfankeji.com/gtftaakgrx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ywan-chungtsiang.top/gtczbfnmad.html

[U103] JS：定时器
来源：http://hz.yj20258.top/gtyzncvwlv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigufen.top/gtteiryzhb.html

[U104] JS：防抖
来源：http://hz.jlsjyb.cn/gtciovcxpd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangdashe.top/gtqlcovzuc.html

[U105] JS：节流
来源：http://hz.ydjk.org.cn/gtjgnkuxbl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinghuilouyu.cn/gtmtijjovq.html

[U106] JS：日期格式化
来源：http://hz.nwbrower.top/gtxawpphhg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258888.top/gtdpomnumk.html

[U107] JS：数字千分位
来源：http://hz.smart0.xyz/gthxvrqqva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.pengpengdd.cyou/gtlssxwvej.html

[U108] JS：随机整数
来源：http://hz.gotoacloud.top/gtyscmpqpn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hnqzz.top/gtkgjbgulc.html

[U109] JS：数组分组
来源：http://hz.yanxiufei.cn/gtwspzwsuw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtdldcards.html

[U110] JS：数组分块
来源：http://hz.shuidangran.top/gtyhmjcktt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hfpthk.cn/gtzrfggopq.html

[U111] JS：对象转 Map
来源：http://hz.cqqwz.cn/gtzxjziwox.html

new Map(Object.entries(obj))
来源：http://hz.andypj.xyz/gtrinmgvfz.html

[U112] JS：字符串补位
来源：http://hz.smart0.xyz/gtaevprite.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtabuvtozg.html

[U113] JS：正则替换全部
来源：http://hz.cqqwz.cn/gtchjapmsr.html

s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtgrggssue.html

[U114] JS：JSON 深比较
来源：http://hz.jinqigufen.top/gtqlzumkdd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxinkj.top/gtzgcsxcff.html

[U115] JS：生成 UUID
来源：http://hz.nanxinkj.top/gtfgnhxdxq.html

crypto.randomUUID()
来源：http://hz.cashguo.top/gtqhwgxnfh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shuidangran.top/gtyzitvqfj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.c1oappe.top/gtqangdows.html

[U117] JS：单元测试
来源：http://hz.tian-w.cn/gtrtnmpxof.html

npm i -D vitest;  npx vitest
来源：http://hz.0kj1m.cn/gtojufplki.html

[U118] JS：开发服务器
来源：http://hz.sxryk.cn/gtrzoanmut.html

npm i -D vite;  npx vite
来源：http://hz.redwolf501.top/gtwzmcyyof.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtffauekts.html

npx vite build
来源：http://hz.chenzaomai.com/gtohtmihno.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yangfankeji.com/gtbsgmzigi.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtnhdgzmph.html

================================================================================
来源：http://hz.redwolf501.top/gtfhwhxvii.html

统计汇总
来源：http://hz.ydzc1.top/gtbxgcvclj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfvcxuout.html

按语言统计（条）：
来源：http://hz.dashuyun.cn/gtzypnvayv.html

Python ......... 252
来源：http://hz.jqgfzy.top/gtauqsvrpg.html

PHP ............ 252
来源：http://hz.hongshengwenyu.top/gthvfgngnb.html

JavaScript ..... 252
来源：http://hz.andypj.xyz/gtajxgzyed.html

TypeScript ..... 212
来源：http://hz.feifeiyinyue.top/gtsjdwldye.html

Java ........... 212
来源：http://hz.yj202588.top/gtdrawhkyo.html

Go ............. 212
来源：http://hz.zhixingplan.top/gtdfytywps.html

Ruby ........... 212
来源：http://hz.yongpay.top/gtoygjchoh.html

C# ............. 212
来源：http://hz.chenzaomai.com/gtfcznnmzl.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtasbglhqs.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtlvqlddac.html

SQL ............ 90
来源：http://hz.316326.xyz/gtncynztib.html

Bash ........... 80
来源：http://hz.nanxuanxn.top/gtnstdtnqb.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtmkappret.html

Swift .......... 15
来源：http://hz.jinyuanbaomall.cn/gtyjsrcycq.html

Lua ............ 10
来源：http://hz.tanke756.top/gtujivfwfr.html

Perl ........... 10
来源：http://hz.svipenyu.cn/gtcylpkspa.html

Scala .......... 10
来源：http://hz.bjfxy.top/gthgxmkpuo.html

------------------------------------
来源：http://hz.jianghu66.top/gtplezbyoc.html

合计 ........... 2106 条
来源：http://hz.jqgufenzy.top/gtvomcrjgj.html

按章节统计：
来源：http://hz.snrcjt.cn/gtwycckjfc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.ywan-chungtsiang.top/gtornytrma.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnqzz.top/gtuojmhmda.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtvgcorbjv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtiujsamvg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtcxnriphv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cheryme.top/gtmjflyanu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cqqwz.cn/gtglffotox.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtqpqenvvn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtuetmnaqj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtjttiqygw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtkkrsjexn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtgkflowgx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtvglyebek.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sufxvd.cn/gtkmsajors.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.iojbl.cn/gtgnkaaaia.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xuanzx.com/gtedlyhxbb.html

Q SQL 专题                              90
来源：http://hz.aizwys.cn/gtcftuxjap.html

R Bash 专题                             80
来源：http://hz.zdqjudy.top/gtkqbedvvq.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtcjcanced.html

T 其他语言补充                          60
来源：http://hz.ivvv.top/gtxdhnfsbq.html

U 高频实用片段                         120
来源：http://hz.cashguo.top/gtrtalxhrj.html

------------------------------------
来源：http://hz.hammf.cn/gtdmwhkazt.html

合计                                  2106 条
来源：http://hz.hnxiangtu.top/gttraiwryy.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtbmwqujyg.html

使用提醒
来源：http://hz.zhoulong.xyz/gthiammjhm.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtjrliycqz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhoulong.xyz/gtnbfoqrnl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenlongwang.top/gtbirqpdsn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.svipenyu.cn/gtnmhlekmm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jinqigfzy.top/gtxkxvxccd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.smart0.xyz/gtxkvahcnd.html

—— 文件结束 ——
来源：http://hz.shanyushiyangkeji.top/gtccynjqlv.html

================================================================================
来源：http://hz.zdqjudy.top/gtihekrrij.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cucudq.cn/gtnguwvknk.html

Common Programming Examples Cheat Book
来源：http://hz.chenzaomai.com/gtxavytxkp.html

================================================================================
来源：http://hz.andypj.xyz/gtzulneprt.html

【收录内容】
来源：http://hz.ybcxt.top/gtjgmxkxcu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.fzhhl.top/gtbecxvlmo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jyoumei.cn/gtqoiqdrni.html

SQL · Bash · C · C++
来源：http://hz.daria6918.cn/gtykmbxajz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zycfv.cn/gtztkvarhq.html

【使用说明】
来源：http://hz.zhixingplan.top/gtunpfvixu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yuanzhike.top/gtgpvoelyt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.316326.xyz/gtelrqboor.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jianghu66.top/gtxcrlfcyh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.daxiang520.top/gttgmmgetc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.haohaochexian.top/gtqolkbpzh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hnqzz.top/gtvslszsfn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yongpay.top/gtcyhyfhxl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fzhhl.top/gtivbdjzfi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.316326.xyz/gtrecpjomf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zycfv.cn/gtfpttrluz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhixingplan.top/gtdjjgiycp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.daxiang520.top/gtfxninpwh.html

【文件统计】
来源：http://hz.shanyushiyangtech.top/gtrzcdgwnn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jlsjyb.cn/gtebkegmao.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtbfvgqkwo.html

目  录
来源：http://hz.redwolf501.top/gtzuopgrip.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtsldcejgh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.tianlin.xyz/gtdprnumvw.html


<!-- 参考信息 -->