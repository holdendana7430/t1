代发 wailian999

case class User(name: String, age: Int)
来源：http://hz.ybcxt.top/gtsuczgpom.html

[T57] Scala：模式匹配
来源：http://hz.hywenlv.cn/gtgleqrzhr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtghkrafkh.html

[T58] Scala：函数定义
来源：http://hz.hfpthk.cn/gtslzozxmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhengqikj.top/gtvgesiupt.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gttnxsgypn.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtwjwjvgea.html

[T60] Scala：折叠
来源：http://hz.nanxinkj.top/gtqdscieis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gtdlgsrzea.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtveuztnwj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gttoyzisaw.html

================================================================================
来源：http://hz.jianghu66.top/gtegbiesjv.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtiegecvqc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.0kj1m.cn/gtccujleal.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxuanxn.top/gtsmuzxlva.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtpcnfyjrm.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtmlfllbit.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinqigfzy.top/gtqyqddzbx.html

[U04] Py：变量调试打印
来源：http://hz.feifeiyinyue.top/gtbiyfxmre.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.birdmap.top/gtfhqvasix.html

[U05] Py：列表去重且保序
来源：http://hz.xingfuxueyuan.xyz/gtuktffewy.html

list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gtjkisgiqw.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtbbsctjig.html

{**a, **b}
来源：http://hz.cdnleiting.top/gtqujxxehi.html

[U07] Py：反转字典键值
来源：http://hz.c1oappe.top/gtigqapoev.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gtjmbqnfsc.html

[U08] Py：展平二维列表
来源：http://hz.sufxvd.cn/gtgnosxory.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gtzxxoypex.html

[U09] Py：字典取最大值的键
来源：http://hz.hnxiangtu.top/gtgwdbdiwz.html

max(d, key=d.get)
来源：http://hz.yj20258888.top/gtumkiopwv.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtwbxujpri.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtjurnmtkc.html

[U11] Py：生成器表达式
来源：http://hz.mhx1999.top/gtbsnxjxaf.html

(x * 2 for x in arr)
来源：http://hz.daria6918.cn/gthnsfmdgf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenlongwang.top/gttghwswov.html

Counter(arr).most_common(3)
来源：http://hz.daria6918.cn/gtkbisoflk.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtjmfbufry.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtgqscabyy.html

[U14] Py：分组收集到列表
来源：http://hz.aizwys.cn/gtpdlyenrl.html

defaultdict(list)
来源：http://hz.sufxvd.cn/gtthvrttzv.html

[U15] Py：高精度计时
来源：http://hz.redwolf501.top/gtiyvevyiv.html

t = time.perf_counter()
来源：http://hz.xuetiantiany.cn/gtrfceegal.html

[U16] Py：命令行参数解析
来源：http://hz.havefunace.top/gtcmksvbay.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.fengsongda.top/gtltgwkzan.html

[U17] Py：初始化日志
来源：http://hz.hnqzz.top/gtjhwdrphz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.9152youxi.cn/gttfhkknhb.html

[U18] Py：预编译正则
来源：http://hz.fengsongda.top/gtdzictlwm.html

pat = re.compile(r"\d+")
来源：http://hz.yj202588.top/gtorykyfpl.html

[U19] Py：正则替换带回调
来源：http://hz.xingfuxueyuan.xyz/gtvceeuguw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtfzrcqxic.html

[U20] Py：缓存函数结果
来源：http://hz.zycfv.cn/gtzxmlinhj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtxwvrxtwk.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gtrvcywocb.html

@contextlib.contextmanager
来源：http://hz.cqqwz.cn/gtfnbwcsak.html

[U22] Py：矩阵转置
来源：http://hz.xuetiantiany.cn/gtqqvcajhv.html

list(zip(*m))
来源：http://hz.havefunace.top/gthtoelfuc.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtczvznyqc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pycfn.com/gtvnhostel.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtinihpiss.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cdnleiting.top/gtkgfztkje.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtyfxeowzp.html

csv.DictReader(f)
来源：http://hz.sufxvd.cn/gtesyvfpff.html

[U26] Py：并发下载
来源：http://hz.tian-w.cn/gtgcmfkrrv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtoqzpcnxf.html

[U27] Py：异步 HTTP
来源：http://hz.ydjk.org.cn/gtfqfpmhnq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtbhjiixcl.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gtmochleyf.html

UserId = int
来源：http://hz.hammf.cn/gtguovgksv.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtugwknusj.html

@property 与 @x.setter 配合
来源：http://hz.sweek.top/gtlqjyhsfn.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtmmcajnxz.html

@dataclass(slots=True)
来源：http://hz.chenjidiqi.icu/gtnsvcnwvh.html

[U31] Py：单测
来源：http://hz.jinqigufen.top/gtrtreyocc.html

python -m pytest -q
来源：http://hz.guowangkeji.top/gtnkowiswi.html

[U32] Py：代码格式化
来源：http://hz.meibo888.top/gtubtpwyom.html

ruff format . && ruff check --fix .
来源：http://hz.ydzc1.top/gtsfvbmvlm.html

[U33] Py：打包发布
来源：http://hz.jianghu66.top/gthqdanzhx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenzaomai.com/gtagytzshe.html

[U34] Py：判断编码
来源：http://hz.feifeiyinyue.top/gtzomzkkib.html

chardet.detect(raw)
来源：http://hz.ivvv.top/gtmcgpvxio.html

[U35] Py：发送邮件
来源：http://hz.daxiang520.top/gtlrxjhbrg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cucudq.cn/gtzrpysydc.html

[U36] Py：定时任务
来源：http://hz.iojbl.cn/gtrvgokioa.html

schedule.every(10).minutes.do(job)
来源：http://hz.gzhubu.top/gtzxzqqdiy.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gtkbsdczar.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gthvigvyrg.html

[U38] Py：获取脚本所在目录
来源：http://hz.yanxiufei.cn/gtnuxyamke.html

Path(__file__).resolve().parent
来源：http://hz.jianghu66.top/gtthoowvdn.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnqzz.top/gtwgqyrmdm.html

sys.stdout.isatty()
来源：http://hz.wangshuangyany.cn/gtanrqkjxq.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gtknbexatc.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtzzwqgryz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.aizwys.cn/gtriecjxxt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yanxiufei.cn/gtkmxnhxzs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.kuanghao11.cn/gtjantxbmx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydjk.org.cn/gtixcabeji.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtfzwkksqa.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtovcfexlk.html

[U44] PHP：开启严格类型
来源：http://hz.redwolf501.top/gtjfcxlmwn.html

declare(strict_types=1);
来源：http://hz.yonumen.top/gtswlhhmcx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tanke756.top/gtvhkibrrw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtgdllmeks.html

[U46] PHP：可空类型
来源：http://hz.zhoulong.xyz/gttdwxambn.html

?string $name = null
来源：http://hz.yonumen.top/gtpsyjglxz.html

[U47] PHP：联合类型
来源：http://hz.sweek.top/gtukaywiww.html

int|string $id
来源：http://hz.jianghu66.top/gtzajukwwe.html

[U48] PHP：纯枚举
来源：http://hz.hongshengwenyu.top/gtgahxnjsv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tanke756.top/gtzygexiex.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtvefquepl.html

public readonly string $name
来源：http://hz.cqqwz.cn/gtlssyndqc.html

[U50] PHP：构造器属性提升
来源：http://hz.shanyushiyangkeji.top/gtsxycdxcg.html

public function __construct(private int $id) {}
来源：http://hz.ydzc1.top/gtqznyzvbn.html

[U51] PHP：数组解构
来源：http://hz.jinyuanbaomall.cn/gtlzjoviis.html

[$a, $b] = $arr;
来源：http://hz.xinyue.icu/gtresskzei.html

[U52] PHP：箭头函数
来源：http://hz.fzhhl.top/gtdiitrvzy.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtmqozidts.html

[U53] PHP：空合并运算符
来源：http://hz.jlsjyb.cn/gtkqgahrfy.html

$v = $a ?? $b ?? "default";
来源：http://hz.zdqjudy.top/gtlwlerjur.html

[U54] PHP：空安全调用
来源：http://hz.zhiwuduotai.top/gtfhmoywus.html

$obj?->method()
来源：http://hz.bjfxy.top/gttzlewepn.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtwjwbsrxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aizwys.cn/gtxbhwytil.html

[U56] PHP：命名参数
来源：http://hz.yangfankeji.com/gtlxwndybn.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtjgiatxpm.html

[U57] PHP：字符串插值
来源：http://hz.zhoulong.xyz/gtcnejwcgk.html

"值: {$a}"
来源：http://hz.shangyingyoupin.top/gtynqxsmnp.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtyobulgpt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sxryk.cn/gteddilxsd.html

[U59] PHP：自定义排序
来源：http://hz.wangshuangyany.cn/gtjgxcpquj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtfkoajhaf.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtkblestrn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhixingplan.top/gtlinobwzk.html

[U61] PHP：正则
来源：http://hz.jinghuilouyu.cn/gtzuarazxp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtrrxzsabg.html

[U62] PHP：日期对象
来源：http://hz.ivvv.top/gtbudbbxmi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.0kj1m.cn/gtfmhrmfbr.html

[U63] PHP：文件读写
来源：http://hz.yvedp.cn/gtqbulfurq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.mhx1999.top/gtluotqaah.html

[U64] PHP：目录遍历
来源：http://hz.cashguo.top/gtmoqfywzx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.fengsongda.top/gtyggghqpt.html

[U65] PHP：会话
来源：http://hz.jqgufenzy.top/gtlsxyxnux.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yangfankeji.com/gtttfzamli.html

[U66] PHP：设置 Cookie
来源：http://hz.sysykeji.top/gtagnvcikk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nanxinkj.top/gtfnjjphcj.html

[U67] PHP：处理文件上传
来源：http://hz.jqgfzy.top/gtmlqagpjo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cashguo.top/gttqpoluxa.html

[U68] PHP：PDO 连接
来源：http://hz.hfpthk.cn/gtsbayvika.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zdqjudy.top/gttlrrfxvu.html

[U69] PHP：PDO 预处理
来源：http://hz.yangfankeji.com/gtzwmktuzz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sxryk.cn/gtafibrxef.html

[U70] PHP：PDO 事务
来源：http://hz.cashguo.top/gtikmpowrq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zycfv.cn/gtuhzzqnnb.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gthsdvvbge.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuetiantiany.cn/gtwczdssaf.html

[U72] PHP：写错误日志
来源：http://hz.zhengqikj.top/gtujlbeesy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.pengpengdd.cyou/gtpikazrin.html

[U73] PHP：读取 ini 配置
来源：http://hz.52xcode.cn/gtiyqkasax.html

parse_ini_file("config.ini", true)
来源：http://hz.nwbrower.top/gtyrehvxxj.html

[U74] PHP：读取环境变量
来源：http://hz.dashuyun.cn/gtfzrdqqdf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtlomnglly.html

[U75] PHP：依赖注入
来源：http://hz.hammf.cn/gtoaoefxmj.html

composer require psr/container
来源：http://hz.zycfv.cn/gtddzujcko.html

[U76] PHP：简单路由
来源：http://hz.pycfn.com/gthqbiexhs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dashuyun.cn/gtjvvodazq.html

[U77] PHP：模板渲染
来源：http://hz.yvedp.cn/gtryvsmvto.html

composer require twig/twig
来源：http://hz.jinqigufen.top/gtoftsuuiy.html

[U78] PHP：单元测试
来源：http://hz.cashguo.top/gtvbnrhqte.html

composer require --dev phpunit/phpunit
来源：http://hz.wangshuangyany.cn/gtgmkzyzug.html

[U79] PHP：静态分析
来源：http://hz.sufxvd.cn/gtnbltpmfq.html

composer require --dev phpstan/phpstan
来源：http://hz.cqqwz.cn/gtnevmkbma.html

[U80] PHP：代码规范修复
来源：http://hz.ppjwa.cn/gtpdnehcwl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xinyue.icu/gtbrhlfgkt.html

[U81] JS：初始化项目
来源：http://hz.cashguo.top/gtxpqpqpoj.html

npm init -y;  npm i express
来源：http://hz.gzhubu.top/gtkzffwihf.html

[U82] JS：package.json 脚本
来源：http://hz.yonumen.top/gtbicwnirs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.aibaodan.cn/gtmdhvfjdf.html

[U83] JS：ES Module 导入导出
来源：http://hz.zycfv.cn/gtvulmbknl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtnscxuavz.html

[U84] JS：CommonJS 写法
来源：http://hz.xinyue.icu/gtxzdjuzlc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.xuetiantiany.cn/gtldqjphnx.html

[U85] JS：可选链
来源：http://hz.birdmap.top/gtygpjpcds.html

a?.b?.c
来源：http://hz.gotoacloud.top/gtalvikitn.html

[U86] JS：空值合并
来源：http://hz.jinqigfzy.top/gtpoisexwe.html

a ?? b
来源：http://hz.tian-w.cn/gthfpuoxcg.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtholufcbj.html

const { a = 1, b = 2 } = obj;
来源：http://hz.0kj1m.cn/gtwuchamaf.html

[U88] JS：对象展开合并
来源：http://hz.zhongyouzk.top/gtcclusqjd.html

{ ...a, ...b }
来源：http://hz.gotoacloud.top/gtsqgfxkzm.html

[U89] JS：数组去重
来源：http://hz.ppjwa.cn/gtfrfzgwzz.html

[...new Set(arr)]
来源：http://hz.sxryk.cn/gttwdygsjr.html

[U90] JS：数字数组排序
来源：http://hz.9152youxi.cn/gtklvjomrx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtvywruxje.html

[U91] JS：对象键值遍历
来源：http://hz.kuanghao11.cn/gtglcnshig.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yongpay.top/gtvszkthrc.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtjdxkyhaf.html

structuredClone(obj)
来源：http://hz.hywenlv.cn/gtfdymrylx.html

[U93] JS：模板字符串
来源：http://hz.jlsjyb.cn/gtxwhaarql.html

`共 ${n} 条`
来源：http://hz.ydjk.org.cn/gtvqbgnkrn.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gthvnzlwdo.html

const double = x => x * 2;
来源：http://hz.wangdashe.top/gtfsznmmii.html

[U95] JS：Promise 包装
来源：http://hz.zhaomingkeji.xyz/gtrfjpoqya.html

new Promise((resolve, reject) => {})
来源：http://hz.cdnleiting.top/gtcpdcokbx.html

[U96] JS：async/await 与异常
来源：http://hz.pycfn.com/gtyxfapvff.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtgiqzyxgm.html

[U97] JS：并发请求
来源：http://hz.yuxming.cn/gtjrgajsbk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtoyqsptcu.html

[U98] JS：fetch 带 JSON
来源：http://hz.ppjwa.cn/gtbbebffkw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hysaishi.cn/gtoahbnujs.html

[U99] JS：事件监听
来源：http://hz.yj20258.top/gtggfdrvvr.html

el.addEventListener("click", e => {})
来源：http://hz.tian-w.cn/gtwsxxousr.html

[U100] JS：DOM 查询
来源：http://hz.yj20258.top/gtqxyaahow.html

document.querySelector(".item")
来源：http://hz.jinqigfzy.top/gtipsadsbc.html

[U101] JS：classList 操作
来源：http://hz.zhijiandao.cn/gtkbgxzefr.html

el.classList.toggle("active")
来源：http://hz.xuetiantiany.cn/gtdncnauri.html

[U102] JS：本地存储
来源：http://hz.jianghu66.top/gtdrvsffij.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.daxiang520.top/gtfsopsydz.html

[U103] JS：定时器
来源：http://hz.yangfankeji.com/gtjojpvmsq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shangyingyoupin.top/gtfbrikylc.html

[U104] JS：防抖
来源：http://hz.zhaomingkeji.xyz/gtjemiyfvg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtmsihbbya.html

[U105] JS：节流
来源：http://hz.ppjwa.cn/gttmrkaiix.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.guannengcc.top/gtgtlencuo.html

[U106] JS：日期格式化
来源：http://hz.aizwys.cn/gtykgamlrg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinqigufen.top/gtmppiauaw.html

[U107] JS：数字千分位
来源：http://hz.fengsongda.top/gtoodjnuav.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtiwykxscd.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtncxswkwx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhoulong.xyz/gtrrxsylkr.html

[U109] JS：数组分组
来源：http://hz.ppjwa.cn/gtvprttkap.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtljoiwbbx.html

[U110] JS：数组分块
来源：http://hz.hnxiangtu.top/gtprtiyatx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhijiandao.cn/gturctrvaz.html

[U111] JS：对象转 Map
来源：http://hz.hammf.cn/gtjggdwqfd.html

new Map(Object.entries(obj))
来源：http://hz.chenjidiqi.icu/gtmdpnospo.html

[U112] JS：字符串补位
来源：http://hz.chenlongwang.top/gtvwuvzfnl.html

"7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtvbrcjvik.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gttpfhscfn.html

s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtbjxbmqph.html

[U114] JS：JSON 深比较
来源：http://hz.andypj.xyz/gtsadrfzpq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangdashe.top/gtquljvysb.html

[U115] JS：生成 UUID
来源：http://hz.shangyingyoupin.top/gtrghebkse.html

crypto.randomUUID()
来源：http://hz.xuanzx.com/gtjoaasyka.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cashguo.top/gtacfbsvtk.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhongyouzk.top/gtneblnkll.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangtech.top/gtntwxqsrg.html

npm i -D vitest;  npx vitest
来源：http://hz.birdmap.top/gtgawkkebq.html

[U118] JS：开发服务器
来源：http://hz.jqgufenzy.top/gtpvzlcvlu.html

npm i -D vite;  npx vite
来源：http://hz.sufxvd.cn/gtxfyxyrsg.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gtjoanamec.html

npx vite build
来源：http://hz.hongshengwenyu.top/gtjxnfvxcn.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xziqi.cn/gtrxyhlamo.html

import.meta.env.VITE_API_URL
来源：http://hz.yongpay.top/gtbfhynygd.html

================================================================================
来源：http://hz.svipenyu.cn/gttzgxumfm.html

统计汇总
来源：http://hz.ydjk.org.cn/gtawtnngfr.html

================================================================================
来源：http://hz.yuanzhike.top/gtcrncbrlv.html

按语言统计（条）：
来源：http://hz.sweek.top/gtnwkswylc.html

Python ......... 252
来源：http://hz.wangdashe.top/gtcmufakiv.html

PHP ............ 252
来源：http://hz.meibo888.top/gtfvujcgey.html

JavaScript ..... 252
来源：http://hz.jqgfzy.top/gtlnwcuguu.html

TypeScript ..... 212
来源：http://hz.yj20258.top/gtqtznpwuu.html

Java ........... 212
来源：http://hz.tanke756.top/gtotvjqmcg.html

Go ............. 212
来源：http://hz.fzhhl.top/gtqgnmtkdm.html

Ruby ........... 212
来源：http://hz.kuanghao11.cn/gtdfkjitzy.html

C# ............. 212
来源：http://hz.fzhhl.top/gtvbhidkwb.html

C .............. 30
来源：http://hz.316326.xyz/gtpurlyniu.html

C++ ............ 30
来源：http://hz.gotoacloud.top/gtmgffpakl.html

SQL ............ 90
来源：http://hz.shanyushiyangkeji.top/gtyxupnuvz.html

Bash ........... 80
来源：http://hz.sysykeji.top/gtwwnolcmo.html

Kotlin ......... 15
来源：http://hz.hysaishi.cn/gtwfettfkz.html

Swift .......... 15
来源：http://hz.jyoumei.cn/gtnmbpswmb.html

Lua ............ 10
来源：http://hz.chenzaomai.com/gtpcpxcjtg.html

Perl ........... 10
来源：http://hz.guannengcc.top/gtnaxvbuze.html

Scala .......... 10
来源：http://hz.pengpengdd.cyou/gtwmcrtfzu.html

------------------------------------
来源：http://hz.nwbrower.top/gtzikxgzai.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtddwcsnpe.html

按章节统计：
来源：http://hz.snrcjt.cn/gtskbfeons.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtevdrrfrg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.guowangkeji.top/gtcyqhiadj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtmeitiqfj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.316326.xyz/gtzhjdkgea.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.vqdsnc.cn/gtyadcqiru.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtlmwaauiv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zdqjudy.top/gtdvalojef.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtwanbkbdl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtrbczkmjt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtwvajqpcg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jiagoushi.top/gtlrktcufa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.guannengcc.top/gtyvfrwsie.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtykrxnzdw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aibaodan.cn/gtbjtdduft.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxuanxn.top/gtmflctyfx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtonigwgee.html

Q SQL 专题                              90
来源：http://hz.ydjk.org.cn/gtuesxscyq.html

R Bash 专题                             80
来源：http://hz.shuidangran.top/gtheprmpca.html

S C / C++ 专题                          60
来源：http://hz.nanxuanxn.top/gttizefhwt.html

T 其他语言补充                          60
来源：http://hz.shzxlz.cn/gtkkuacxig.html

U 高频实用片段                         120
来源：http://hz.zhijiandao.cn/gtnaelmxjq.html

------------------------------------
来源：http://hz.yuanzhike.top/gtdtbauvqx.html

合计                                  2106 条
来源：http://hz.xingfuxueyuan.xyz/gtsdkqkhfu.html

--------------------------------------------------------------------------------
来源：http://hz.sufxvd.cn/gtfeymzkzh.html


<!-- 参考信息 -->