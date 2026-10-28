代发 wailian999

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtmsxvsqaf.html

[T53] Scala：字符串插值
来源：http://hz.sysykeji.top/gtcvppmwxx.html

s"值: $b"
来源：http://hz.hongshengwenyu.top/gtybrzdmgw.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtyojijsji.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nwbrower.top/gtcdaguhky.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtzylhcyps.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtawynhqjn.html

[T56] Scala：样例类
来源：http://hz.pycfn.com/gtcsdjubyk.html

case class User(name: String, age: Int)
来源：http://hz.ybcxt.top/gtrpacbqfx.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtxxqsuhpe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtfwixtddl.html

[T58] Scala：函数定义
来源：http://hz.gzhubu.top/gtpggdlaoq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhaomingkeji.xyz/gtcqsetagw.html

[T59] Scala：循环
来源：http://hz.fzhhl.top/gthtvrlckd.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigufen.top/gtnpbmhgmj.html

[T60] Scala：折叠
来源：http://hz.vqdsnc.cn/gtqgktlthe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtrdlrtjkr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtlmkwdahz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtqtxvomol.html

================================================================================
来源：http://hz.ivvv.top/gtaccsfuoh.html

[U01] Py：创建虚拟环境
来源：http://hz.ydjk.org.cn/gtalbexmgi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtudnwufmu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtmoamoohv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigfzy.top/gtobfoilyu.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtbyiseyye.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgufenzy.top/gtrrmrymng.html

[U04] Py：变量调试打印
来源：http://hz.zhengqikj.top/gtznkbifsp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.haohaochexian.top/gtjkxybcwn.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtspjfglau.html

list(dict.fromkeys(arr))
来源：http://hz.sweek.top/gtvahbzmuo.html

[U06] Py：合并两个字典
来源：http://hz.yangfankeji.com/gtdhhbaddw.html

{**a, **b}
来源：http://hz.shanyushiyangtech.top/gtkdpxvwkq.html

[U07] Py：反转字典键值
来源：http://hz.jinghuilouyu.cn/gtdrhjdczn.html

{v: k for k, v in d.items()}
来源：http://hz.chenjidiqi.icu/gtcxxmikty.html

[U08] Py：展平二维列表
来源：http://hz.yj20258.top/gtdrwldnfl.html

[y for x in nested for y in x]
来源：http://hz.chenzaomai.com/gttljbhaiq.html

[U09] Py：字典取最大值的键
来源：http://hz.fzhhl.top/gtejxdxraj.html

max(d, key=d.get)
来源：http://hz.gotoacloud.top/gtcrmjwbfv.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangtech.top/gtbqdtmdjc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gtzutotgpz.html

[U11] Py：生成器表达式
来源：http://hz.xylfe.cn/gtmspbljyi.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gtfnqxedrk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.bjfxy.top/gtmnqydhmj.html

Counter(arr).most_common(3)
来源：http://hz.yanxiufei.cn/gtdoqaecvk.html

[U13] Py：固定长度队列
来源：http://hz.jlsjyb.cn/gtxbshfogd.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtqvdrfbei.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtmcxuaztj.html

defaultdict(list)
来源：http://hz.haohaochexian.top/gthoijvjru.html

[U15] Py：高精度计时
来源：http://hz.zhixingplan.top/gthtwhxngm.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtccwbfdci.html

[U16] Py：命令行参数解析
来源：http://hz.ppjwa.cn/gtzthuviym.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jyoumei.cn/gtnbafmvpk.html

[U17] Py：初始化日志
来源：http://hz.jlsjyb.cn/gtxwyvnrzn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.quarkkingdee.top/gtnzrdzwdv.html

[U18] Py：预编译正则
来源：http://hz.0kj1m.cn/gtwqzbwrcj.html

pat = re.compile(r"\d+")
来源：http://hz.havefunace.top/gttomhwxsd.html

[U19] Py：正则替换带回调
来源：http://hz.aizwys.cn/gtkmcajqjy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydjk.org.cn/gtjcewgszn.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gtvtyofdyd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenjidiqi.icu/gtqihkjnqw.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtzlbksqvg.html

@contextlib.contextmanager
来源：http://hz.316326.xyz/gtvybdmapw.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtwusszdza.html

list(zip(*m))
来源：http://hz.jianghu66.top/gtlpqnympv.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gthhrlnqin.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gaohongyu789.top/gtqessnftx.html

[U24] Py：路径操作
来源：http://hz.zhiwuduotai.top/gtsjzypfvu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhixingplan.top/gtngwceumf.html

[U25] Py：CSV 按字典读
来源：http://hz.52xcode.cn/gtrwsoueln.html

csv.DictReader(f)
来源：http://hz.yueranfly.top/gtionvhyhi.html

[U26] Py：并发下载
来源：http://hz.shzxlz.cn/gtqfmdcdzy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtqpsuovct.html

[U27] Py：异步 HTTP
来源：http://hz.kuanghao11.cn/gtmlrcgzrw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shzxlz.cn/gtoqtzvwer.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtlglkriqm.html

UserId = int
来源：http://hz.jianghu66.top/gtpliakjep.html

[U29] Py：属性校验
来源：http://hz.52xcode.cn/gtzewqgmxl.html

@property 与 @x.setter 配合
来源：http://hz.yueranfly.top/gtwkmdpcwp.html

[U30] Py：数据类
来源：http://hz.quarkkingdee.top/gtoychmyuo.html

@dataclass(slots=True)
来源：http://hz.gzhubu.top/gtjcixrlab.html

[U31] Py：单测
来源：http://hz.shzxlz.cn/gtexarakrm.html

python -m pytest -q
来源：http://hz.shanyushiyangtech.top/gtdvbfxglq.html

[U32] Py：代码格式化
来源：http://hz.daria6918.cn/gtagpulsaf.html

ruff format . && ruff check --fix .
来源：http://hz.yonumen.top/gtfnqkfhsp.html

[U33] Py：打包发布
来源：http://hz.iojbl.cn/gtrafuzofc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtljcawffj.html

[U34] Py：判断编码
来源：http://hz.jyoumei.cn/gtkhhklsoo.html

chardet.detect(raw)
来源：http://hz.cashguo.top/gtrckqcqsk.html

[U35] Py：发送邮件
来源：http://hz.jinyuanbaomall.cn/gtnehcajch.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jiagoushi.top/gtjrfprlwi.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtizlrypld.html

schedule.every(10).minutes.do(job)
来源：http://hz.shzxlz.cn/gtybboouwj.html

[U37] Py：读写 Excel
来源：http://hz.yj20258888.top/gtucynjpsl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenlongwang.top/gtzbjzljmu.html

[U38] Py：获取脚本所在目录
来源：http://hz.meibo888.top/gtsfdvjvlj.html

Path(__file__).resolve().parent
来源：http://hz.ydjk.org.cn/gtngeutubw.html

[U39] Py：判断是否在交互环境
来源：http://hz.yanxiufei.cn/gtghzmlvoq.html

sys.stdout.isatty()
来源：http://hz.guowangkeji.top/gtitbdhkru.html

[U40] Py：打印到标准错误
来源：http://hz.yj202588.top/gtsuzjvajp.html

print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtxcyqyjgw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gogol.net.cn/gtmjtpxqlv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.snrcjt.cn/gtqyspcsxu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhaomingkeji.xyz/gtztcccnuw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ywan-chungtsiang.top/gtairxpyvi.html

[U43] PHP：声明命名空间
来源：http://hz.havefunace.top/gtozhgemex.html

namespace App\Http;
来源：http://hz.yanxiufei.cn/gtrnqketnc.html

[U44] PHP：开启严格类型
来源：http://hz.pycfn.com/gtydmwfecn.html

declare(strict_types=1);
来源：http://hz.jinghuilouyu.cn/gtesifkmkm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fengsongda.top/gtannthsjn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtrihfhvoi.html

[U46] PHP：可空类型
来源：http://hz.hysaishi.cn/gtkozrugfd.html

?string $name = null
来源：http://hz.yj202588.top/gtnsywfpvz.html

[U47] PHP：联合类型
来源：http://hz.aizwys.cn/gtqjdrhguk.html

int|string $id
来源：http://hz.jyoumei.cn/gtrkerbxjk.html

[U48] PHP：纯枚举
来源：http://hz.ehwqpu.com/gtqacxglhk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhixingplan.top/gtebabhxvi.html

[U49] PHP：只读属性
来源：http://hz.meibo888.top/gtbujghwtf.html

public readonly string $name
来源：http://hz.fzhhl.top/gtqwghaikb.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtdfwmqzcn.html

public function __construct(private int $id) {}
来源：http://hz.pycfn.com/gtfymlzscr.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtiuzwjtgw.html

[$a, $b] = $arr;
来源：http://hz.zdqjudy.top/gtaxzkxmzo.html

[U52] PHP：箭头函数
来源：http://hz.hongshengwenyu.top/gtbswvfqoe.html

$double = fn($x) => $x * 2;
来源：http://hz.bjfxy.top/gtyqlxqqgj.html

[U53] PHP：空合并运算符
来源：http://hz.jinyuanbaomall.cn/gttfpkkjxu.html

$v = $a ?? $b ?? "default";
来源：http://hz.dianchejie.cn/gtnavogmmj.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtosvtbade.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gtennxaptr.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gtphhvxini.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtoolwhaag.html

[U56] PHP：命名参数
来源：http://hz.feifeiyinyue.top/gtvkgyrnkq.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtnytvhzch.html

[U57] PHP：字符串插值
来源：http://hz.wangdashe.top/gtgsaqsmpx.html

"值: {$a}"
来源：http://hz.bjfxy.top/gtxhmshrsh.html

[U58] PHP：数组三件套
来源：http://hz.shanyushiyangtech.top/gtcwjfpaby.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.guannengcc.top/gtjmrgjgog.html

[U59] PHP：自定义排序
来源：http://hz.cheryme.top/gtnartmzig.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtwiumzzdu.html

[U60] PHP：JSON 编解码
来源：http://hz.xylfe.cn/gtrwptgxdx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sxryk.cn/gttwrgrhxz.html

[U61] PHP：正则
来源：http://hz.daxiang520.top/gtfwitszzk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtqggdyovp.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtuxwwedhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gthbovmyly.html

[U63] PHP：文件读写
来源：http://hz.xinyue.icu/gtmlidhqyc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtepscktgm.html

[U64] PHP：目录遍历
来源：http://hz.mhx1999.top/gtcuhkcnec.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hongshengwenyu.top/gtjkwxleih.html

[U65] PHP：会话
来源：http://hz.yj20258888.top/gtjfgqeysc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hnxiangtu.top/gtualchbkt.html

[U66] PHP：设置 Cookie
来源：http://hz.yongpay.top/gtqbxagevt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hysaishi.cn/gthvqeqywp.html

[U67] PHP：处理文件上传
来源：http://hz.bjfxy.top/gthyymzdpf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ybcxt.top/gtflbchgjw.html

[U68] PHP：PDO 连接
来源：http://hz.yanxiufei.cn/gtxeoqgcnt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.snrcjt.cn/gtdtddblgt.html

[U69] PHP：PDO 预处理
来源：http://hz.snrcjt.cn/gtcqjgbcaw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hongshengwenyu.top/gtgkqkeeyc.html

[U70] PHP：PDO 事务
来源：http://hz.9152youxi.cn/gtgbzewaqc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuetiantiany.cn/gttdhpavbx.html

[U71] PHP：抛出异常
来源：http://hz.52xcode.cn/gtaunekkke.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtmtecprgs.html

[U72] PHP：写错误日志
来源：http://hz.birdmap.top/gttgbdwghy.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yvedp.cn/gtpkwotyyo.html

[U73] PHP：读取 ini 配置
来源：http://hz.nanxuanxn.top/gtcbzhnrpl.html

parse_ini_file("config.ini", true)
来源：http://hz.daxiang520.top/gtffdrkdcx.html

[U74] PHP：读取环境变量
来源：http://hz.cucudq.cn/gtxrulvhub.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ybcxt.top/gtnmldaszw.html

[U75] PHP：依赖注入
来源：http://hz.nanxinkj.top/gteogucofc.html

composer require psr/container
来源：http://hz.shuidangran.top/gtrflexwzo.html

[U76] PHP：简单路由
来源：http://hz.52xcode.cn/gtglarscwd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.zhaomingkeji.xyz/gtqadfqjrj.html

[U77] PHP：模板渲染
来源：http://hz.jlsjyb.cn/gtpwoawetk.html

composer require twig/twig
来源：http://hz.sufxvd.cn/gtkjzserml.html

[U78] PHP：单元测试
来源：http://hz.chenlongwang.top/gtszlvivua.html

composer require --dev phpunit/phpunit
来源：http://hz.tanke756.top/gtdmdsejsp.html

[U79] PHP：静态分析
来源：http://hz.wangdashe.top/gtxnehmrso.html

composer require --dev phpstan/phpstan
来源：http://hz.ydjk.org.cn/gtmdmcyofq.html

[U80] PHP：代码规范修复
来源：http://hz.yonumen.top/gtbfyjludh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jyoumei.cn/gtobmrlhzh.html

[U81] JS：初始化项目
来源：http://hz.andypj.xyz/gtclyxduon.html

npm init -y;  npm i express
来源：http://hz.ppjwa.cn/gtkjbywgap.html

[U82] JS：package.json 脚本
来源：http://hz.tanke756.top/gtkbaomapk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.tian-w.cn/gtazsczmrn.html

[U83] JS：ES Module 导入导出
来源：http://hz.hnxiangtu.top/gtpcgtuoxu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jqgfzy.top/gtdlrohwhn.html

[U84] JS：CommonJS 写法
来源：http://hz.xylfe.cn/gtcsgasjmh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shanyushiyangkeji.top/gtqtjkiqmh.html

[U85] JS：可选链
来源：http://hz.redwolf501.top/gtwgoovgbe.html

a?.b?.c
来源：http://hz.hnqzz.top/gtgwhzvsjm.html

[U86] JS：空值合并
来源：http://hz.andypj.xyz/gtnrwknfiy.html

a ?? b
来源：http://hz.wangdashe.top/gtfgqnztkv.html

[U87] JS：解构默认值
来源：http://hz.meibo888.top/gtpbikndug.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guowangkeji.top/gtkmqlqdko.html

[U88] JS：对象展开合并
来源：http://hz.52xcode.cn/gtvedbxczd.html

{ ...a, ...b }
来源：http://hz.mhx1999.top/gtyvhkvfpi.html

[U89] JS：数组去重
来源：http://hz.jlsjyb.cn/gtyklrsloc.html

[...new Set(arr)]
来源：http://hz.gotoacloud.top/gtkqlxxmac.html

[U90] JS：数字数组排序
来源：http://hz.smart0.xyz/gtgprtjwjb.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtlmjhnavt.html

[U91] JS：对象键值遍历
来源：http://hz.ydzc1.top/gttxledvjx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yongpay.top/gtgvvldkbp.html

[U92] JS：深拷贝
来源：http://hz.yanxiufei.cn/gtqnswrdlh.html

structuredClone(obj)
来源：http://hz.yongpay.top/gtaascpilh.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtnvksjqqd.html

`共 ${n} 条`
来源：http://hz.0kj1m.cn/gtrxrtwrhv.html

[U94] JS：箭头函数
来源：http://hz.chenzaomai.com/gtlhxxfpth.html

const double = x => x * 2;
来源：http://hz.wangshuangyany.cn/gtwdajhono.html

[U95] JS：Promise 包装
来源：http://hz.cheryme.top/gtghqelarx.html

new Promise((resolve, reject) => {})
来源：http://hz.xuetiantiany.cn/gtcrmrziub.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtplqyrfmq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gttxzvmbmd.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtclkmmgfx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gthklmtlpl.html

[U98] JS：fetch 带 JSON
来源：http://hz.yanxiufei.cn/gtdptrynaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxuanxn.top/gtxbchduwb.html

[U99] JS：事件监听
来源：http://hz.ehwqpu.com/gtuvswascx.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gtsvxcqsjk.html

[U100] JS：DOM 查询
来源：http://hz.tanke756.top/gtnijufznm.html

document.querySelector(".item")
来源：http://hz.ydzc1.top/gtbplbetpv.html

[U101] JS：classList 操作
来源：http://hz.iojbl.cn/gtebzrnqwh.html

el.classList.toggle("active")
来源：http://hz.bjfxy.top/gtgthjfqcz.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtpojttgrr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ivvv.top/gtivxyouro.html

[U103] JS：定时器
来源：http://hz.chenlongwang.top/gtfiubescv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.hysaishi.cn/gtktacmlbl.html

[U104] JS：防抖
来源：http://hz.ivvv.top/gtxddcnvtg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtiptbmnys.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtgjidaodq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yj20258888.top/gtgwhqgfbh.html

[U106] JS：日期格式化
来源：http://hz.yuxming.cn/gtvbayowud.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.316326.xyz/gtvnuuicls.html

[U107] JS：数字千分位
来源：http://hz.yuanzhike.top/gtchgqrxmh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gotoacloud.top/gtilfsvhop.html

[U108] JS：随机整数
来源：http://hz.guowangkeji.top/gtjoyszjwq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gtlzqvpxym.html

[U109] JS：数组分组
来源：http://hz.zhengqikj.top/gtiuqaqwpu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.smart0.xyz/gtkdbjrhtd.html

[U110] JS：数组分块
来源：http://hz.yvedp.cn/gtkoaftvbw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.guannengcc.top/gtsqiqyzfz.html

[U111] JS：对象转 Map
来源：http://hz.0kj1m.cn/gtjxfaahsm.html

new Map(Object.entries(obj))
来源：http://hz.zhongyouzk.top/gtvzuqhszm.html

[U112] JS：字符串补位
来源：http://hz.shzxlz.cn/gtkhvhtzzh.html

"7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtxryzwcbd.html

[U113] JS：正则替换全部
来源：http://hz.tianlin.xyz/gtjflflzlq.html

s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtkqqdvitw.html

[U114] JS：JSON 深比较
来源：http://hz.dashuyun.cn/gtefnxakqp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtswrrotgd.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gtmbqrihds.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtstmenjjb.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtgxwavrhc.html

/** @param {string} name */ function f(name) {}
来源：http://hz.0kj1m.cn/gtcxgzlovr.html

[U117] JS：单元测试
来源：http://hz.tianlin.xyz/gtiveiqfpt.html

npm i -D vitest;  npx vitest
来源：http://hz.chenlongwang.top/gtvavdnftn.html

[U118] JS：开发服务器
来源：http://hz.jyoumei.cn/gtugcydwfj.html

npm i -D vite;  npx vite
来源：http://hz.yuanzhike.top/gtwyjjucbt.html

[U119] JS：生产构建
来源：http://hz.yangfankeji.com/gtvwredcuk.html

npx vite build
来源：http://hz.jinghuilouyu.cn/gtisgwckpd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gttvcqwysq.html

import.meta.env.VITE_API_URL
来源：http://hz.jinqigufen.top/gtronypmyc.html

================================================================================
来源：http://hz.hywenlv.cn/gtmflwxgnx.html

统计汇总
来源：http://hz.gzhubu.top/gttgzuvbgo.html

================================================================================
来源：http://hz.cdnleiting.top/gtqittgfyx.html

按语言统计（条）：
来源：http://hz.chenlongwang.top/gtovreotls.html

Python ......... 252
来源：http://hz.svipenyu.cn/gtbnfdmjgc.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtydwygjbe.html

JavaScript ..... 252
来源：http://hz.redwolf501.top/gtfjevwixq.html

TypeScript ..... 212
来源：http://hz.fengsongda.top/gtucqnngsb.html

Java ........... 212
来源：http://hz.tianlin.xyz/gtokmfwchm.html

Go ............. 212
来源：http://hz.gaohongyu789.top/gtoyjwdmgj.html

Ruby ........... 212
来源：http://hz.wangshuangyany.cn/gthwnkqemx.html

C# ............. 212
来源：http://hz.ybcxt.top/gtpnkrxfsz.html

C .............. 30
来源：http://hz.shuidangran.top/gtcjurgduu.html

C++ ............ 30
来源：http://hz.ywan-chungtsiang.top/gtonawmmhu.html

SQL ............ 90
来源：http://hz.aibaodan.cn/gtvsfgzngp.html

Bash ........... 80
来源：http://hz.yongpay.top/gtdlsyxwjq.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtocivdyby.html

Swift .......... 15
来源：http://hz.nanxuanxn.top/gtmbbqnyrt.html

Lua ............ 10
来源：http://hz.yuxming.cn/gthtuolutn.html

Perl ........... 10
来源：http://hz.gaohongyu789.top/gtwqittcnc.html

Scala .......... 10
来源：http://hz.nanxuanxn.top/gtddhmvuwo.html

------------------------------------
来源：http://hz.cashguo.top/gtvpmebpxy.html

合计 ........... 2106 条
来源：http://hz.hongshengwenyu.top/gtengrjutd.html

按章节统计：
来源：http://hz.pycfn.com/gtimwczpld.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtgksxdezq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtdaopixat.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtkjnzcfxo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.cheryme.top/gthritlign.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.fengsongda.top/gtxogfmdyn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhaomingkeji.xyz/gtuhwkiwfq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtjabvytwr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhongyouzk.top/gtzlbzmtpk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtwrghgunn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zdqjudy.top/gtsoqqlzbn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtcffwynly.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtlfkpiucc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gtluieasls.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nwbrower.top/gtcmxienqd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.wangshuangyany.cn/gtuaholdto.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jinqigufen.top/gturpzkkvv.html


<!-- 参考信息 -->