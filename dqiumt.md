代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuxming.cn/gtwtmiutyc.html

[T59] Scala：循环
来源：http://hz.gogol.net.cn/gtwzapocvs.html

for (i <- 1 to 10) println(i)
来源：http://hz.vqdsnc.cn/gtzhxwlcub.html

[T60] Scala：折叠
来源：http://hz.smart0.xyz/gtnkxvcdrn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtebkdkkip.html

================================================================================
来源：http://hz.daria6918.cn/gtzcfcqryg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.redwolf501.top/gtowtfarxb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdnysvoyr.html

[U01] Py：创建虚拟环境
来源：http://hz.jiagoushi.top/gtjlkgedli.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.mhx1999.top/gtatnvkhyk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnqzz.top/gtdvwfddqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yvedp.cn/gtkutvkdpe.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtvgvkedsj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gtulkkympj.html

[U04] Py：变量调试打印
来源：http://hz.jinghuilouyu.cn/gtbrfsnido.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hongshengwenyu.top/gthfibicxm.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtzcsqboiy.html

list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtpvjlbguq.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtxnldeniq.html

{**a, **b}
来源：http://hz.dianchejie.cn/gthctjcavh.html

[U07] Py：反转字典键值
来源：http://hz.bjfxy.top/gtbdnfgrtz.html

{v: k for k, v in d.items()}
来源：http://hz.wangdashe.top/gtsoqiroxm.html

[U08] Py：展平二维列表
来源：http://hz.zhongyouzk.top/gtnxgrinuy.html

[y for x in nested for y in x]
来源：http://hz.cheryme.top/gttcyoqsxz.html

[U09] Py：字典取最大值的键
来源：http://hz.cucudq.cn/gtctjwdpvf.html

max(d, key=d.get)
来源：http://hz.hywenlv.cn/gttkliisiu.html

[U10] Py：按值排序字典
来源：http://hz.nwbrower.top/gtjakensje.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258.top/gtoiugydzd.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtsokucofx.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gtpcplaijk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.snrcjt.cn/gtcrjzkvdn.html

Counter(arr).most_common(3)
来源：http://hz.xuetiantiany.cn/gtpvondnyp.html

[U13] Py：固定长度队列
来源：http://hz.zhiwuduotai.top/gtcvyuecmr.html

deque(maxlen=10)
来源：http://hz.xinyue.icu/gtrtcoocdw.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtyvsqeuqe.html

defaultdict(list)
来源：http://hz.wangdashe.top/gtzkvpuboh.html

[U15] Py：高精度计时
来源：http://hz.gzhubu.top/gtnlioblln.html

t = time.perf_counter()
来源：http://hz.jinqigfzy.top/gteeulucri.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtigdmceso.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xinyue.icu/gtxrdwhldv.html

[U17] Py：初始化日志
来源：http://hz.zdqjudy.top/gtlibgprrw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ehwqpu.com/gtojmrlknx.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtykxnrvzv.html

pat = re.compile(r"\d+")
来源：http://hz.c1oappe.top/gtcsfjwbid.html

[U19] Py：正则替换带回调
来源：http://hz.tian-w.cn/gtvehseavb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangkeji.top/gtdncibvfe.html

[U20] Py：缓存函数结果
来源：http://hz.bjfxy.top/gtpxjdcqiy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtketvueel.html

[U21] Py：自定义上下文管理器
来源：http://hz.mhx1999.top/gtmliqabct.html

@contextlib.contextmanager
来源：http://hz.daria6918.cn/gtafhstxef.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtlvmanriu.html

list(zip(*m))
来源：http://hz.aibaodan.cn/gtrrkkunlq.html

[U23] Py：分块读取大文件
来源：http://hz.chenjidiqi.icu/gttxzalicr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ppjwa.cn/gtsehfdhfj.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtibqzqbeg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuxming.cn/gtynflklzm.html

[U25] Py：CSV 按字典读
来源：http://hz.ivvv.top/gttafztnys.html

csv.DictReader(f)
来源：http://hz.zhoulong.xyz/gtwinrqyqk.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtdvlduaut.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.smart0.xyz/gtkngarfrv.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtgzpzdfbk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gtiybwtrcj.html

[U28] Py：类型别名
来源：http://hz.zhixingplan.top/gtgkdaasyl.html

UserId = int
来源：http://hz.ybcxt.top/gtmpsrjvgg.html

[U29] Py：属性校验
来源：http://hz.birdmap.top/gtnvazcqaz.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtcdecbidg.html

[U30] Py：数据类
来源：http://hz.yj20258.top/gtjomdcfpi.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtfyqeognm.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtghbmfjxt.html

python -m pytest -q
来源：http://hz.guowangkeji.top/gtrbylclgj.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtbwhigqiu.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtiggfjfex.html

[U33] Py：打包发布
来源：http://hz.andypj.xyz/gtsgawkgpk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258.top/gtjufkozwz.html

[U34] Py：判断编码
来源：http://hz.ybcxt.top/gtyckkakpk.html

chardet.detect(raw)
来源：http://hz.zhongyouzk.top/gtbyzeafhr.html

[U35] Py：发送邮件
来源：http://hz.chenjidiqi.icu/gthjrzkudp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.iojbl.cn/gtmicnbkxf.html

[U36] Py：定时任务
来源：http://hz.gzhubu.top/gtbwmkhdrp.html

schedule.every(10).minutes.do(job)
来源：http://hz.52xcode.cn/gtzulwjjdz.html

[U37] Py：读写 Excel
来源：http://hz.shuidangran.top/gtmisvemmw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gtugouippr.html

[U38] Py：获取脚本所在目录
来源：http://hz.cdnleiting.top/gtbminnemj.html

Path(__file__).resolve().parent
来源：http://hz.yangfankeji.com/gtnfeludhu.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtqsonptrf.html

sys.stdout.isatty()
来源：http://hz.dianchejie.cn/gtzswvgnnt.html

[U40] Py：打印到标准错误
来源：http://hz.dashuyun.cn/gtxsjlludf.html

print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtclflngiz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sweek.top/gtkbtrekpz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ppjwa.cn/gthvrdrcnc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gtfybiznmc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ehwqpu.com/gtvhcjptna.html

[U43] PHP：声明命名空间
来源：http://hz.havefunace.top/gtpwthdogm.html

namespace App\Http;
来源：http://hz.xylfe.cn/gtqlqvgywo.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtlynnocrj.html

declare(strict_types=1);
来源：http://hz.kuanghao11.cn/gthtccdkjh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258.top/gtjlvksnlg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtaawwujfl.html

[U46] PHP：可空类型
来源：http://hz.zdqjudy.top/gtixeszpxu.html

?string $name = null
来源：http://hz.snrcjt.cn/gtdhlnmbln.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtadhpkeir.html

int|string $id
来源：http://hz.jiagoushi.top/gtotvxwuuw.html

[U48] PHP：纯枚举
来源：http://hz.guannengcc.top/gtkgumgsin.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gaohongyu789.top/gtalnmvegs.html

[U49] PHP：只读属性
来源：http://hz.hnqzz.top/gtyaqjysum.html

public readonly string $name
来源：http://hz.xziqi.cn/gtrjnkdmrs.html

[U50] PHP：构造器属性提升
来源：http://hz.aibaodan.cn/gtstxzxnrr.html

public function __construct(private int $id) {}
来源：http://hz.redwolf501.top/gtytctuqtq.html

[U51] PHP：数组解构
来源：http://hz.aizwys.cn/gtmnvvzhoq.html

[$a, $b] = $arr;
来源：http://hz.xuetiantiany.cn/gtfcfbchuz.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtonmrggyu.html

$double = fn($x) => $x * 2;
来源：http://hz.yj202588.top/gtsczxtipw.html

[U53] PHP：空合并运算符
来源：http://hz.jinyuanbaomall.cn/gtwcpywdey.html

$v = $a ?? $b ?? "default";
来源：http://hz.cdnleiting.top/gtrnxpqmsa.html

[U54] PHP：空安全调用
来源：http://hz.jianghu66.top/gtiqckzjai.html

$obj?->method()
来源：http://hz.andypj.xyz/gtuydjxjwt.html

[U55] PHP：match 表达式
来源：http://hz.guowangkeji.top/gtqfuqouwa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gtztbxmaow.html

[U56] PHP：命名参数
来源：http://hz.shangyingyoupin.top/gtncpyfjfn.html

f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gtyztovrxn.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gtcpfafohc.html

"值: {$a}"
来源：http://hz.svipenyu.cn/gtaesrrxvo.html

[U58] PHP：数组三件套
来源：http://hz.cheryme.top/gtigohxljo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gtjhpazbth.html

[U59] PHP：自定义排序
来源：http://hz.birdmap.top/gtwmzjiapr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gthbjfxmfu.html

[U60] PHP：JSON 编解码
来源：http://hz.xuanzx.com/gtzbrxtyja.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shuidangran.top/gtwpqrdrpd.html

[U61] PHP：正则
来源：http://hz.chenzaomai.com/gtmwztqrqi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtjwlxacae.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gtjwtrdcus.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenzaomai.com/gtxavbqlch.html

[U63] PHP：文件读写
来源：http://hz.cqqwz.cn/gtbhhfpaxa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xylfe.cn/gtflljgawf.html

[U64] PHP：目录遍历
来源：http://hz.haohaochexian.top/gtrqnumqgc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.birdmap.top/gtpmbdfsns.html

[U65] PHP：会话
来源：http://hz.mhx1999.top/gtwgbmhoep.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ivvv.top/gtozjkcpir.html

[U66] PHP：设置 Cookie
来源：http://hz.aizwys.cn/gtqpzyhhae.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jianghu66.top/gtbothnpav.html

[U67] PHP：处理文件上传
来源：http://hz.dashuyun.cn/gtgphplone.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yuxming.cn/gtqoqsroxt.html

[U68] PHP：PDO 连接
来源：http://hz.xylfe.cn/gtcgwckrsk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ydzc1.top/gtzdusslwx.html

[U69] PHP：PDO 预处理
来源：http://hz.zhiwuduotai.top/gtsvtwvggn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtxzygjumf.html

[U70] PHP：PDO 事务
来源：http://hz.jiagoushi.top/gtjynbzuyx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.kuanghao11.cn/gtssgesabs.html

[U71] PHP：抛出异常
来源：http://hz.yuxming.cn/gtbsdbvvqi.html

throw new RuntimeException("失败", 500);
来源：http://hz.birdmap.top/gtuswcilso.html

[U72] PHP：写错误日志
来源：http://hz.yuxming.cn/gtwhbznmht.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hywenlv.cn/gtjmpjyvsr.html

[U73] PHP：读取 ini 配置
来源：http://hz.cucudq.cn/gtirzpfbyc.html

parse_ini_file("config.ini", true)
来源：http://hz.sysykeji.top/gtryubcgjq.html

[U74] PHP：读取环境变量
来源：http://hz.ppjwa.cn/gttlcegool.html

getenv("APP_ENV") ?: "production"
来源：http://hz.quarkkingdee.top/gtlygfvdsc.html

[U75] PHP：依赖注入
来源：http://hz.zhoulong.xyz/gtqezhniud.html

composer require psr/container
来源：http://hz.hammf.cn/gtrcnbxgcf.html

[U76] PHP：简单路由
来源：http://hz.aizwys.cn/gtjakelrkc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.meibo888.top/gtbtpdyvkj.html

[U77] PHP：模板渲染
来源：http://hz.cashguo.top/gtixyhrmbx.html

composer require twig/twig
来源：http://hz.shangyingyoupin.top/gtlayfvihg.html

[U78] PHP：单元测试
来源：http://hz.quarkkingdee.top/gtjmotlghr.html

composer require --dev phpunit/phpunit
来源：http://hz.jqgufenzy.top/gtpsxntgwa.html

[U79] PHP：静态分析
来源：http://hz.wangshuangyany.cn/gtqvczdmnm.html

composer require --dev phpstan/phpstan
来源：http://hz.cucudq.cn/gtomelyzmk.html

[U80] PHP：代码规范修复
来源：http://hz.yongpay.top/gtaqowhzog.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.aizwys.cn/gtelgbkeza.html

[U81] JS：初始化项目
来源：http://hz.nwbrower.top/gtyxhhfabh.html

npm init -y;  npm i express
来源：http://hz.nwbrower.top/gtploweowe.html

[U82] JS：package.json 脚本
来源：http://hz.xylfe.cn/gtbxphtuix.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.cucudq.cn/gtvvbwlacl.html

[U83] JS：ES Module 导入导出
来源：http://hz.vqdsnc.cn/gtngrbliav.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtjugaagdj.html

[U84] JS：CommonJS 写法
来源：http://hz.feifeiyinyue.top/gtdssmcmdj.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhixingplan.top/gtajohmacp.html

[U85] JS：可选链
来源：http://hz.quarkkingdee.top/gtrtmgmtzt.html

a?.b?.c
来源：http://hz.yj20258888.top/gtjjkxtrsc.html

[U86] JS：空值合并
来源：http://hz.nanxuanxn.top/gtbyicspfm.html

a ?? b
来源：http://hz.daria6918.cn/gtsglncycu.html

[U87] JS：解构默认值
来源：http://hz.gzhubu.top/gtppklgcmr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.smart0.xyz/gtbqirolwa.html

[U88] JS：对象展开合并
来源：http://hz.wangdashe.top/gtbgzccmah.html

{ ...a, ...b }
来源：http://hz.daria6918.cn/gtlnpyceao.html

[U89] JS：数组去重
来源：http://hz.dianchejie.cn/gtjhjtnoup.html

[...new Set(arr)]
来源：http://hz.yuxming.cn/gtitgbcmwj.html

[U90] JS：数字数组排序
来源：http://hz.hysaishi.cn/gterztgbrc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtaclsqjwp.html

[U91] JS：对象键值遍历
来源：http://hz.jqgufenzy.top/gtjasqahnz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jyoumei.cn/gtkempydne.html

[U92] JS：深拷贝
来源：http://hz.jinqigfzy.top/gtroavjzqa.html

structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtqdddpega.html

[U93] JS：模板字符串
来源：http://hz.birdmap.top/gtutdubdaa.html

`共 ${n} 条`
来源：http://hz.daria6918.cn/gtxnflkiwx.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtntcwscsd.html

const double = x => x * 2;
来源：http://hz.andypj.xyz/gtwsymewuh.html

[U95] JS：Promise 包装
来源：http://hz.yj202588.top/gtschkdqsf.html

new Promise((resolve, reject) => {})
来源：http://hz.chenzaomai.com/gtskidiuup.html

[U96] JS：async/await 与异常
来源：http://hz.dianchejie.cn/gttqusyksw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gthajiegaq.html

[U97] JS：并发请求
来源：http://hz.9152youxi.cn/gtmaasagen.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtxsaerooh.html

[U98] JS：fetch 带 JSON
来源：http://hz.yuxming.cn/gtgmhdythk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ppjwa.cn/gtbkakuuzp.html

[U99] JS：事件监听
来源：http://hz.xziqi.cn/gtfevbytxg.html

el.addEventListener("click", e => {})
来源：http://hz.chenlongwang.top/gtmydxkcle.html

[U100] JS：DOM 查询
来源：http://hz.yueranfly.top/gtmrknnuab.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtanthnfzz.html

[U101] JS：classList 操作
来源：http://hz.yuanzhike.top/gtdaqgqexj.html

el.classList.toggle("active")
来源：http://hz.jqgufenzy.top/gtfixmnxma.html

[U102] JS：本地存储
来源：http://hz.gzhubu.top/gtjmtdkeka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.bjfxy.top/gtqnpolnqd.html

[U103] JS：定时器
来源：http://hz.kuanghao11.cn/gtqtgvavqb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aizwys.cn/gtnwfvbasv.html

[U104] JS：防抖
来源：http://hz.yangfankeji.com/gtyledianr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtyvxdkddx.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gttydscexu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenzaomai.com/gttlbvgwoc.html

[U106] JS：日期格式化
来源：http://hz.jyoumei.cn/gtsypsqxik.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zdqjudy.top/gtpdejyeiw.html

[U107] JS：数字千分位
来源：http://hz.guannengcc.top/gttoqwylnr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gtffeswdvq.html

[U108] JS：随机整数
来源：http://hz.sysykeji.top/gtydefjenf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.9152youxi.cn/gtlmahqtwu.html

[U109] JS：数组分组
来源：http://hz.meibo888.top/gtzqessllw.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtttvisohl.html

[U110] JS：数组分块
来源：http://hz.yj20258.top/gtdlbhazii.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.smart0.xyz/gtjbjbehjb.html

[U111] JS：对象转 Map
来源：http://hz.cucudq.cn/gtvnqncxnh.html

new Map(Object.entries(obj))
来源：http://hz.ydzc1.top/gtvnlhasjs.html

[U112] JS：字符串补位
来源：http://hz.yanxiufei.cn/gtbdulyegl.html

"7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtusazjgce.html

[U113] JS：正则替换全部
来源：http://hz.ppjwa.cn/gtsrjelazu.html

s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtuxpivwva.html

[U114] JS：JSON 深比较
来源：http://hz.hysaishi.cn/gtmcefmesw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtdbmujptf.html

[U115] JS：生成 UUID
来源：http://hz.sysykeji.top/gtjltajlxb.html

crypto.randomUUID()
来源：http://hz.ivvv.top/gtbehezlct.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shuidangran.top/gtcoewkitu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xylfe.cn/gtwumtazff.html

[U117] JS：单元测试
来源：http://hz.gaohongyu789.top/gtoqxiefku.html

npm i -D vitest;  npx vitest
来源：http://hz.yuanzhike.top/gtzzsemrnk.html

[U118] JS：开发服务器
来源：http://hz.zhijiandao.cn/gtbcxtswea.html

npm i -D vite;  npx vite
来源：http://hz.fengsongda.top/gtunebrohr.html

[U119] JS：生产构建
来源：http://hz.jlsjyb.cn/gtpslnqtcs.html

npx vite build
来源：http://hz.fzhhl.top/gtwkrnrguw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtitmzzssi.html

import.meta.env.VITE_API_URL
来源：http://hz.yuxming.cn/gtflwolegl.html

================================================================================
来源：http://hz.sufxvd.cn/gthaheklrz.html

统计汇总
来源：http://hz.wangshuangyany.cn/gtvjqyhmpw.html

================================================================================
来源：http://hz.hammf.cn/gtkvyfyszg.html

按语言统计（条）：
来源：http://hz.yanxiufei.cn/gtddtgnwfh.html

Python ......... 252
来源：http://hz.feifeiyinyue.top/gtfndxmynw.html

PHP ............ 252
来源：http://hz.zdqjudy.top/gtrpkajapk.html

JavaScript ..... 252
来源：http://hz.cashguo.top/gtyhipqbpc.html

TypeScript ..... 212
来源：http://hz.dianchejie.cn/gtsunyoxym.html

Java ........... 212
来源：http://hz.hnxiangtu.top/gtltebbtzp.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtuegmydnr.html

Ruby ........... 212
来源：http://hz.xuanzx.com/gtnelbljie.html

C# ............. 212
来源：http://hz.ydzc1.top/gtelrjitpm.html

C .............. 30
来源：http://hz.sysykeji.top/gtnbwxnije.html

C++ ............ 30
来源：http://hz.wangdashe.top/gtrgbzskwj.html

SQL ............ 90
来源：http://hz.aizwys.cn/gtugnjgruu.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtprvejjbg.html

Kotlin ......... 15
来源：http://hz.jinqigufen.top/gtcausfwgb.html

Swift .......... 15
来源：http://hz.tian-w.cn/gtqbgckwlj.html

Lua ............ 10
来源：http://hz.dashuyun.cn/gtyznvdbfm.html

Perl ........... 10
来源：http://hz.wangshuangyany.cn/gtpswrfciu.html

Scala .......... 10
来源：http://hz.yuanzhike.top/gtdewdjpiq.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtajnevkiz.html

合计 ........... 2106 条
来源：http://hz.ppjwa.cn/gtesqbmiqb.html

按章节统计：
来源：http://hz.aizwys.cn/gtkfinvfhd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gtbybugbyz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtakhlkgqc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtsglxgesn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtriejbror.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hammf.cn/gtmkqsnesd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtcvlkwklo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtktxoglpx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtvhlcrgwx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sufxvd.cn/gtruklbfra.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gtvrckyobh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shangyingyoupin.top/gtfxncrlpq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.smart0.xyz/gtunkpbxpe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtbovpssxm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.c1oappe.top/gtbqcywbdg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.bjfxy.top/gtuuoidybx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtgqraqybw.html

Q SQL 专题                              90
来源：http://hz.aizwys.cn/gtvdywsckp.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtagjwhjak.html

S C / C++ 专题                          60
来源：http://hz.mhx1999.top/gtzdrylqtj.html

T 其他语言补充                          60
来源：http://hz.xylfe.cn/gtecyxvvwa.html

U 高频实用片段                         120
来源：http://hz.cdnleiting.top/gtrisxfsax.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtmoonyqxf.html

合计                                  2106 条
来源：http://hz.pengpengdd.cyou/gtqwvfyxvm.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gthzzxlpef.html

使用提醒
来源：http://hz.tanke756.top/gtidjbwdnb.html

--------------------------------------------------------------------------------
来源：http://hz.haohaochexian.top/gtylkmgsum.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zdqjudy.top/gtkfpphtkj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.pengpengdd.cyou/gtclsbmpvh.html


<!-- 参考信息 -->