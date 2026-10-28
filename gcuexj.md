代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.yuxming.cn/gtydbaqhpv.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtyewefuje.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dianchejie.cn/gtouycujog.html

[T58] Scala：函数定义
来源：http://hz.birdmap.top/gtfcevfwfp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenzaomai.com/gtuluuszni.html

[T59] Scala：循环
来源：http://hz.guannengcc.top/gtyhupmflg.html

for (i <- 1 to 10) println(i)
来源：http://hz.shangyingyoupin.top/gtpsipzuzq.html

[T60] Scala：折叠
来源：http://hz.hnqzz.top/gtweejasio.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.c1oappe.top/gtofllbkhn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtggkdsfph.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtwqrxquuf.html

================================================================================
来源：http://hz.zhengqikj.top/gtcaesgmia.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtyypsfgwz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtxmuucdep.html

[U02] Py：导出 / 安装依赖
来源：http://hz.svipenyu.cn/gtiaymktmh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtwtbhdhjd.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtvjwschsg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenlongwang.top/gttzsbphet.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gtlbiratlb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtzfltinrh.html

[U05] Py：列表去重且保序
来源：http://hz.vqdsnc.cn/gtdzfcmsro.html

list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtyiwgdjrq.html

[U06] Py：合并两个字典
来源：http://hz.ydjk.org.cn/gtayjeqvrb.html

{**a, **b}
来源：http://hz.havefunace.top/gtvsefbpiv.html

[U07] Py：反转字典键值
来源：http://hz.yj202588.top/gtpzuvbyfe.html

{v: k for k, v in d.items()}
来源：http://hz.shanyushiyangkeji.top/gtutfvcoob.html

[U08] Py：展平二维列表
来源：http://hz.gotoacloud.top/gtoynkcumt.html

[y for x in nested for y in x]
来源：http://hz.iojbl.cn/gtptnqtmzr.html

[U09] Py：字典取最大值的键
来源：http://hz.aizwys.cn/gtndfxfdiq.html

max(d, key=d.get)
来源：http://hz.jianghu66.top/gtoknpmpds.html

[U10] Py：按值排序字典
来源：http://hz.chenlongwang.top/gtnjrtkhom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtbpdsznsy.html

[U11] Py：生成器表达式
来源：http://hz.hywenlv.cn/gtvnbqwlkh.html

(x * 2 for x in arr)
来源：http://hz.cheryme.top/gtqxgdxywu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gtqyhtcyrv.html

Counter(arr).most_common(3)
来源：http://hz.feifeiyinyue.top/gtfwtoobwf.html

[U13] Py：固定长度队列
来源：http://hz.daria6918.cn/gtqkicesbf.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtryvdyejf.html

[U14] Py：分组收集到列表
来源：http://hz.zhixingplan.top/gtooppptdv.html

defaultdict(list)
来源：http://hz.xingfuxueyuan.xyz/gthwqsdlvt.html

[U15] Py：高精度计时
来源：http://hz.aibaodan.cn/gtwnqrvsgv.html

t = time.perf_counter()
来源：http://hz.jinqigufen.top/gtsiwfkkdb.html

[U16] Py：命令行参数解析
来源：http://hz.bjfxy.top/gtsighygfp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnqzz.top/gtfajqxuuq.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gteshxhalv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxuanxn.top/gtogbnszvc.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtvtuufqjv.html

pat = re.compile(r"\d+")
来源：http://hz.hnxiangtu.top/gtbweqbqen.html

[U19] Py：正则替换带回调
来源：http://hz.shuidangran.top/gtnthqyohc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gtsddjdlng.html

[U20] Py：缓存函数结果
来源：http://hz.xingfuxueyuan.xyz/gtpbbkgsit.html

@functools.lru_cache(maxsize=None)
来源：http://hz.pycfn.com/gtyerodgzd.html

[U21] Py：自定义上下文管理器
来源：http://hz.gzhubu.top/gtqfiautco.html

@contextlib.contextmanager
来源：http://hz.jianghu66.top/gtyfucajfi.html

[U22] Py：矩阵转置
来源：http://hz.chenzaomai.com/gtjfbrifot.html

list(zip(*m))
来源：http://hz.bjfxy.top/gtmmgopkyc.html

[U23] Py：分块读取大文件
来源：http://hz.kuanghao11.cn/gthccqhpgh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hongshengwenyu.top/gtkqikyxlm.html

[U24] Py：路径操作
来源：http://hz.haohaochexian.top/gttchxqlno.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtvotrtpax.html

[U25] Py：CSV 按字典读
来源：http://hz.zhongyouzk.top/gtamnuzxri.html

csv.DictReader(f)
来源：http://hz.tanke756.top/gtqjtmgtbj.html

[U26] Py：并发下载
来源：http://hz.nanxinkj.top/gtrrpkrmps.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gaohongyu789.top/gtdsxlpskq.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtwurjjbhg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinghuilouyu.cn/gtqlpqvwuw.html

[U28] Py：类型别名
来源：http://hz.svipenyu.cn/gtvbpqfyjb.html

UserId = int
来源：http://hz.zhoulong.xyz/gtmdnnxjis.html

[U29] Py：属性校验
来源：http://hz.hnqzz.top/gttfaoveka.html

@property 与 @x.setter 配合
来源：http://hz.shanyushiyangkeji.top/gtwhzjfbkg.html

[U30] Py：数据类
来源：http://hz.jlsjyb.cn/gtjqodrzhb.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtlstdgaqw.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtuahwrypb.html

python -m pytest -q
来源：http://hz.havefunace.top/gtwzchuiup.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gtdvxskfwl.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtxbhxuudu.html

[U33] Py：打包发布
来源：http://hz.shzxlz.cn/gtyvimdxmy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jyoumei.cn/gtqlcjpynf.html

[U34] Py：判断编码
来源：http://hz.gaohongyu789.top/gtplbexilx.html

chardet.detect(raw)
来源：http://hz.xinyue.icu/gtbzffalyd.html

[U35] Py：发送邮件
来源：http://hz.yanxiufei.cn/gtifvcybhh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yvedp.cn/gtsykbztpn.html

[U36] Py：定时任务
来源：http://hz.xylfe.cn/gtojbjsjcp.html

schedule.every(10).minutes.do(job)
来源：http://hz.shuidangran.top/gtjsehgghf.html

[U37] Py：读写 Excel
来源：http://hz.hysaishi.cn/gtqoiwlivz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.smart0.xyz/gtcczuidcs.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenlongwang.top/gtizvaitpa.html

Path(__file__).resolve().parent
来源：http://hz.guowangkeji.top/gtptfrorfh.html

[U39] Py：判断是否在交互环境
来源：http://hz.cdnleiting.top/gtwtpkjzkb.html

sys.stdout.isatty()
来源：http://hz.yj202588.top/gterzigjve.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtesjssbhm.html

print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtthieovlr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gtjwlqrpbo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgfzy.top/gtursincpq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hammf.cn/gtuhbzjbew.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xinyue.icu/gtxuksixla.html

[U43] PHP：声明命名空间
来源：http://hz.pycfn.com/gtcelboigu.html

namespace App\Http;
来源：http://hz.cdnleiting.top/gtlyecikiv.html

[U44] PHP：开启严格类型
来源：http://hz.shzxlz.cn/gtoetxkblv.html

declare(strict_types=1);
来源：http://hz.kuanghao11.cn/gthswlyojk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.vqdsnc.cn/gtsjijjwkn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtqoabewnv.html

[U46] PHP：可空类型
来源：http://hz.chenjidiqi.icu/gtvmtyvhmw.html

?string $name = null
来源：http://hz.dashuyun.cn/gtqnfsraxu.html

[U47] PHP：联合类型
来源：http://hz.9152youxi.cn/gtzbynsamt.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtwhjypfij.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtnhjbsrqo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhengqikj.top/gtpayzqcjz.html

[U49] PHP：只读属性
来源：http://hz.ybcxt.top/gtncimpggk.html

public readonly string $name
来源：http://hz.daria6918.cn/gtqvnnyorj.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtbsawkgns.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangkeji.top/gtgurdcpra.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtyxugjsnw.html

[$a, $b] = $arr;
来源：http://hz.52xcode.cn/gtltgfcfpg.html

[U52] PHP：箭头函数
来源：http://hz.fengsongda.top/gtcmjsvmas.html

$double = fn($x) => $x * 2;
来源：http://hz.smart0.xyz/gtstereowa.html

[U53] PHP：空合并运算符
来源：http://hz.chenlongwang.top/gtxdfwubjk.html

$v = $a ?? $b ?? "default";
来源：http://hz.hfpthk.cn/gtmjtgmbxf.html

[U54] PHP：空安全调用
来源：http://hz.zhengqikj.top/gtuxkrcnih.html

$obj?->method()
来源：http://hz.sysykeji.top/gtzcowntgt.html

[U55] PHP：match 表达式
来源：http://hz.smart0.xyz/gtidmfcplw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sxryk.cn/gtefvehkgg.html

[U56] PHP：命名参数
来源：http://hz.hnqzz.top/gtknctuwmt.html

f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtvacegazh.html

[U57] PHP：字符串插值
来源：http://hz.fzhhl.top/gtuwncntvt.html

"值: {$a}"
来源：http://hz.chenjidiqi.icu/gtfacroqkc.html

[U58] PHP：数组三件套
来源：http://hz.smart0.xyz/gtlchbhoky.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhongyouzk.top/gtdbggfwlc.html

[U59] PHP：自定义排序
来源：http://hz.ybcxt.top/gtriptonpb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtptwxbrbx.html

[U60] PHP：JSON 编解码
来源：http://hz.pycfn.com/gtfeaapvwz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ppjwa.cn/gtvudjyvtg.html

[U61] PHP：正则
来源：http://hz.jyoumei.cn/gtpkiygloc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gthxhbbbfc.html

[U62] PHP：日期对象
来源：http://hz.sysykeji.top/gtrpmpbyvo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.52xcode.cn/gtmlfgpwrk.html

[U63] PHP：文件读写
来源：http://hz.zhixingplan.top/gtofbotggn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.sufxvd.cn/gteqjfnmtb.html

[U64] PHP：目录遍历
来源：http://hz.cdnleiting.top/gtcsfmsgbb.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gzhubu.top/gtqxqdbngu.html

[U65] PHP：会话
来源：http://hz.tian-w.cn/gtpeqfowig.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.quarkkingdee.top/gtaowlvbcv.html

[U66] PHP：设置 Cookie
来源：http://hz.nwbrower.top/gtxrfsntkr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydjk.org.cn/gtytxrxxcq.html

[U67] PHP：处理文件上传
来源：http://hz.gogol.net.cn/gtbjabipvt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhongyouzk.top/gtucbhpxca.html

[U68] PHP：PDO 连接
来源：http://hz.fzhhl.top/gtrpaycmrf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yongpay.top/gtywidtyck.html

[U69] PHP：PDO 预处理
来源：http://hz.jiagoushi.top/gtwjmpllls.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gthcdwfriz.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigufen.top/gtnsrwynlx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cashguo.top/gtojyhjglm.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtyxfusvua.html

throw new RuntimeException("失败", 500);
来源：http://hz.fzhhl.top/gtawsnxtez.html

[U72] PHP：写错误日志
来源：http://hz.yanxiufei.cn/gtaejcdjzl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.xylfe.cn/gtdducqlmj.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangtech.top/gtpclqzrih.html

parse_ini_file("config.ini", true)
来源：http://hz.hfpthk.cn/gtdnxaumpa.html

[U74] PHP：读取环境变量
来源：http://hz.hnqzz.top/gttkzttkjj.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jinyuanbaomall.cn/gtcxnhpwhq.html

[U75] PHP：依赖注入
来源：http://hz.9152youxi.cn/gtbizkfeuf.html

composer require psr/container
来源：http://hz.yj20258888.top/gtwjwsqlfy.html

[U76] PHP：简单路由
来源：http://hz.ivvv.top/gtruresmqz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jinghuilouyu.cn/gttdvyopqt.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gttwkxmooj.html

composer require twig/twig
来源：http://hz.jlsjyb.cn/gtoqnjskut.html

[U78] PHP：单元测试
来源：http://hz.shzxlz.cn/gtubwmwiyo.html

composer require --dev phpunit/phpunit
来源：http://hz.bjfxy.top/gtlwrftuyg.html

[U79] PHP：静态分析
来源：http://hz.andypj.xyz/gtgqjletig.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtrphxoaug.html

[U80] PHP：代码规范修复
来源：http://hz.guannengcc.top/gttkulfgdy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.meibo888.top/gtabrsutyw.html

[U81] JS：初始化项目
来源：http://hz.sufxvd.cn/gtlohxkdyk.html

npm init -y;  npm i express
来源：http://hz.zhoulong.xyz/gtiiwfakdf.html

[U82] JS：package.json 脚本
来源：http://hz.xuetiantiany.cn/gttxdoaoyq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sufxvd.cn/gtqayxysdc.html

[U83] JS：ES Module 导入导出
来源：http://hz.c1oappe.top/gtjmaaxuht.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenlongwang.top/gtzdrczcdm.html

[U84] JS：CommonJS 写法
来源：http://hz.fzhhl.top/gtmrrqukuk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sysykeji.top/gtdmmhzcdg.html

[U85] JS：可选链
来源：http://hz.guowangkeji.top/gtkghwkduj.html

a?.b?.c
来源：http://hz.yuanzhike.top/gthmqjhdqn.html

[U86] JS：空值合并
来源：http://hz.pycfn.com/gtpanosqnc.html

a ?? b
来源：http://hz.hammf.cn/gtdstrfkun.html

[U87] JS：解构默认值
来源：http://hz.ywan-chungtsiang.top/gthuxyrlgu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gogol.net.cn/gttjrwftrf.html

[U88] JS：对象展开合并
来源：http://hz.chenzaomai.com/gtftprmtmz.html

{ ...a, ...b }
来源：http://hz.andypj.xyz/gtyqbgqrea.html

[U89] JS：数组去重
来源：http://hz.vqdsnc.cn/gtsjbxglab.html

[...new Set(arr)]
来源：http://hz.ehwqpu.com/gtdwsowjdw.html

[U90] JS：数字数组排序
来源：http://hz.birdmap.top/gtcbpxavaa.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtmoyexkfk.html

[U91] JS：对象键值遍历
来源：http://hz.nanxinkj.top/gttmuuaavh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.9152youxi.cn/gtcabsvqzq.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangtech.top/gtniucdlyg.html

structuredClone(obj)
来源：http://hz.c1oappe.top/gtfveylkwi.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gtjvghyfoj.html

`共 ${n} 条`
来源：http://hz.ehwqpu.com/gtrhytbssq.html

[U94] JS：箭头函数
来源：http://hz.ppjwa.cn/gtvpktvgll.html

const double = x => x * 2;
来源：http://hz.xinyue.icu/gtzjurnwdx.html

[U95] JS：Promise 包装
来源：http://hz.xingfuxueyuan.xyz/gtrbfwusgy.html

new Promise((resolve, reject) => {})
来源：http://hz.havefunace.top/gtzusnzrrt.html

[U96] JS：async/await 与异常
来源：http://hz.xylfe.cn/gtzzhefhoo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtyjwtnyzp.html

[U97] JS：并发请求
来源：http://hz.xuanzx.com/gtubgnauev.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtbnrqqdlh.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhixingplan.top/gtbkktojtl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xziqi.cn/gtabgbzbbp.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtaoqvghyv.html

el.addEventListener("click", e => {})
来源：http://hz.hywenlv.cn/gtpbximovq.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtygowphhk.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtxhxekbsj.html

[U101] JS：classList 操作
来源：http://hz.yanxiufei.cn/gtkfndrqze.html

el.classList.toggle("active")
来源：http://hz.pycfn.com/gtzdtpowil.html

[U102] JS：本地存储
来源：http://hz.yvedp.cn/gtderaddyn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yj202588.top/gtxrsfhztd.html

[U103] JS：定时器
来源：http://hz.xylfe.cn/gtswsgddcl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hammf.cn/gtrplrpxhm.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gtmorjgoqz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtvwqfqcvq.html

[U105] JS：节流
来源：http://hz.guannengcc.top/gttmcvghrs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.kuanghao11.cn/gtpcxxczgl.html

[U106] JS：日期格式化
来源：http://hz.ydjk.org.cn/gtujykygzu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigufen.top/gthkdkjqcl.html

[U107] JS：数字千分位
来源：http://hz.svipenyu.cn/gtkhmofeup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhixingplan.top/gtnshrjztt.html

[U108] JS：随机整数
来源：http://hz.yj20258888.top/gtuxisiccb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shzxlz.cn/gtxmcutulz.html

[U109] JS：数组分组
来源：http://hz.snrcjt.cn/gtscptiqak.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtiyvxreib.html

[U110] JS：数组分块
来源：http://hz.andypj.xyz/gtyucqtsma.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigfzy.top/gtxghrimsh.html

[U111] JS：对象转 Map
来源：http://hz.yongpay.top/gtfjyepmjd.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtglbomyal.html

[U112] JS：字符串补位
来源：http://hz.0kj1m.cn/gtzuzqrnem.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gttvyvvrge.html

[U113] JS：正则替换全部
来源：http://hz.fzhhl.top/gtggcvibgl.html

s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtzzfdqgsr.html

[U114] JS：JSON 深比较
来源：http://hz.fzhhl.top/gtmvpzvdva.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtaroovpbs.html

[U115] JS：生成 UUID
来源：http://hz.meibo888.top/gtylerfoey.html

crypto.randomUUID()
来源：http://hz.ydzc1.top/gtuvanhgoz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ywan-chungtsiang.top/gtfygzsxla.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuanzx.com/gttdubjrjt.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtksedkyyd.html

npm i -D vitest;  npx vitest
来源：http://hz.pycfn.com/gtgvnchhky.html

[U118] JS：开发服务器
来源：http://hz.ywan-chungtsiang.top/gtouuwnyin.html

npm i -D vite;  npx vite
来源：http://hz.redwolf501.top/gthqacobcs.html

[U119] JS：生产构建
来源：http://hz.tianlin.xyz/gtgvnqvgpl.html

npx vite build
来源：http://hz.daria6918.cn/gttmscjruq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.iojbl.cn/gtfdepjmzk.html

import.meta.env.VITE_API_URL
来源：http://hz.ivvv.top/gtjizdzhon.html

================================================================================
来源：http://hz.wangdashe.top/gtmuwijanp.html

统计汇总
来源：http://hz.nwbrower.top/gtwyvjvknu.html

================================================================================
来源：http://hz.daxiang520.top/gtmejmipee.html

按语言统计（条）：
来源：http://hz.redwolf501.top/gtiuossstm.html

Python ......... 252
来源：http://hz.kuanghao11.cn/gtokdgzdan.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtqathvwgz.html

JavaScript ..... 252
来源：http://hz.yangfankeji.com/gtsvqrrwhp.html

TypeScript ..... 212
来源：http://hz.gzhubu.top/gtuillsjws.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtogznlzsj.html

Go ............. 212
来源：http://hz.9152youxi.cn/gtitruprwe.html

Ruby ........... 212
来源：http://hz.jiagoushi.top/gtxnqvulec.html

C# ............. 212
来源：http://hz.vqdsnc.cn/gtmdkuwlvu.html

C .............. 30
来源：http://hz.ywan-chungtsiang.top/gtanlueqes.html

C++ ............ 30
来源：http://hz.chenzaomai.com/gtmnrejsyc.html

SQL ............ 90
来源：http://hz.zhongyouzk.top/gtnxryjyhu.html

Bash ........... 80
来源：http://hz.shanyushiyangtech.top/gtoyecftee.html

Kotlin ......... 15
来源：http://hz.zhoulong.xyz/gtecakbldt.html

Swift .......... 15
来源：http://hz.shzxlz.cn/gtyjpsbyvg.html

Lua ............ 10
来源：http://hz.xuetiantiany.cn/gtaxobboaf.html

Perl ........... 10
来源：http://hz.gotoacloud.top/gtmjjifncv.html

Scala .......... 10
来源：http://hz.aizwys.cn/gtspgspdsl.html

------------------------------------
来源：http://hz.jinqigfzy.top/gtyqozpniv.html

合计 ........... 2106 条
来源：http://hz.pengpengdd.cyou/gtwkhnichw.html

按章节统计：
来源：http://hz.cdnleiting.top/gtoekhatax.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.feifeiyinyue.top/gtdsdwvxpn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hnxiangtu.top/gtdtlrozen.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtuojkbbaw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtynxhqrlw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shuidangran.top/gtcbpbczpr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tian-w.cn/gtthtdfdmw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtauwqehhh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hywenlv.cn/gtqkcqfeny.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtcirrpqif.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtiygjfeya.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtsaeaprdg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtkwmzexek.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtdxovkofv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.guowangkeji.top/gtdegvoyqd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sxryk.cn/gtworblodz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtzrwilloo.html

Q SQL 专题                              90
来源：http://hz.bjfxy.top/gtvzvsrrha.html

R Bash 专题                             80
来源：http://hz.52xcode.cn/gtqptanzhe.html

S C / C++ 专题                          60
来源：http://hz.dianchejie.cn/gttzrsodac.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtgmwadazr.html

U 高频实用片段                         120
来源：http://hz.yueranfly.top/gtxhvtpbts.html

------------------------------------
来源：http://hz.yj20258888.top/gtfokfogny.html

合计                                  2106 条
来源：http://hz.jinghuilouyu.cn/gtmudxjfwu.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtybkkhdwm.html


<!-- 参考信息 -->