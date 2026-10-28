代发 wailian999

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtvrnhtrbn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtdhsnkplx.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtxmwlummi.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gtnieqigao.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gtiaanppxy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtmvzupims.html

[T50] Perl：逐行读文件
来源：http://hz.andypj.xyz/gttrnmvlxt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtnyklnvsz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtwmrpjwjn.html

[T51] Scala：Hello World
来源：http://hz.tianlin.xyz/gtmpgshgzm.html

println("Hello")
来源：http://hz.cdnleiting.top/gthixontdm.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtotawdaxs.html

val a = 1;  var b = 2
来源：http://hz.bjfxy.top/gtygbloagz.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtburhyfoo.html

s"值: $b"
来源：http://hz.tian-w.cn/gtvsfwegzt.html

[T54] Scala：集合映射
来源：http://hz.jyoumei.cn/gtkktdhnsd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sxryk.cn/gtmrafsnxt.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtjqdmhlaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shuidangran.top/gtunviuvjl.html

[T56] Scala：样例类
来源：http://hz.daxiang520.top/gteaoovxkg.html

case class User(name: String, age: Int)
来源：http://hz.meibo888.top/gtgrpacsfs.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtzrzwkrhw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtarhcblcp.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtxsgcxmxz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tianlin.xyz/gthfsojqil.html

[T59] Scala：循环
来源：http://hz.yongpay.top/gtbgmaddtg.html

for (i <- 1 to 10) println(i)
来源：http://hz.fengsongda.top/gttegxyzdu.html

[T60] Scala：折叠
来源：http://hz.gaohongyu789.top/gthnwraqpk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tian-w.cn/gtxyfcimor.html

================================================================================
来源：http://hz.nwbrower.top/gtqeowtyhp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtsnlnhnzi.html

================================================================================
来源：http://hz.316326.xyz/gtllolhuov.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtvrknecar.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ivvv.top/gtdzcyiddq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ehwqpu.com/gtlblnefkv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daria6918.cn/gtsaamikma.html

[U03] Py：加载 .env 配置
来源：http://hz.ppjwa.cn/gtsjeqpjgg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ywan-chungtsiang.top/gtljjxmktr.html

[U04] Py：变量调试打印
来源：http://hz.gaohongyu789.top/gttsgqfbaw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cqqwz.cn/gthidxkkff.html

[U05] Py：列表去重且保序
来源：http://hz.haohaochexian.top/gtoqtmgfdv.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtfapgnzxa.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtgsnbjmcv.html

{**a, **b}
来源：http://hz.aizwys.cn/gtlugckodn.html

[U07] Py：反转字典键值
来源：http://hz.nanxinkj.top/gtczobgmki.html

{v: k for k, v in d.items()}
来源：http://hz.daxiang520.top/gtizlxtgwk.html

[U08] Py：展平二维列表
来源：http://hz.jiagoushi.top/gtlrcazdoi.html

[y for x in nested for y in x]
来源：http://hz.hywenlv.cn/gtcuukjujx.html

[U09] Py：字典取最大值的键
来源：http://hz.hfpthk.cn/gtsqglqtcn.html

max(d, key=d.get)
来源：http://hz.hnxiangtu.top/gtrebiwjwp.html

[U10] Py：按值排序字典
来源：http://hz.kuanghao11.cn/gtaupyfvob.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnxiangtu.top/gtwacopziu.html

[U11] Py：生成器表达式
来源：http://hz.fengsongda.top/gtihivyisp.html

(x * 2 for x in arr)
来源：http://hz.shanyushiyangtech.top/gtiwruqhdx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ywan-chungtsiang.top/gtmergrvyo.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtzfozkhbs.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtqeubghkx.html

deque(maxlen=10)
来源：http://hz.yangfankeji.com/gthjsmgkst.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gthqiowfyz.html

defaultdict(list)
来源：http://hz.vqdsnc.cn/gticoeepyu.html

[U15] Py：高精度计时
来源：http://hz.shuidangran.top/gtzarstjnv.html

t = time.perf_counter()
来源：http://hz.guannengcc.top/gtflasgfsg.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtifavicrk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.bjfxy.top/gtmxffohjs.html

[U17] Py：初始化日志
来源：http://hz.nanxinkj.top/gtafkknwnc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gttodczddg.html

[U18] Py：预编译正则
来源：http://hz.yj20258.top/gtijjoibbm.html

pat = re.compile(r"\d+")
来源：http://hz.jqgufenzy.top/gtbwfsoypy.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtoadgfsny.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangkeji.top/gtnqssvubz.html

[U20] Py：缓存函数结果
来源：http://hz.aibaodan.cn/gtxyfaymau.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtitnncrpu.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtubzacuyn.html

@contextlib.contextmanager
来源：http://hz.guannengcc.top/gtiaqdqiwn.html

[U22] Py：矩阵转置
来源：http://hz.fengsongda.top/gtaqcfftrp.html

list(zip(*m))
来源：http://hz.mhx1999.top/gtrkbttqbi.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtefvgcngo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinqigfzy.top/gtrcmxmffw.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtjnecxaay.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.pycfn.com/gtrdlqewic.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtgwjcozuf.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gtewbmithf.html

[U26] Py：并发下载
来源：http://hz.xingfuxueyuan.xyz/gtdvekpxni.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yanxiufei.cn/gtufduzeku.html

[U27] Py：异步 HTTP
来源：http://hz.xziqi.cn/gtxzwdsisa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zycfv.cn/gtottghool.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtjofphqfb.html

UserId = int
来源：http://hz.guowangkeji.top/gtcnfffobu.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtaivntmux.html

@property 与 @x.setter 配合
来源：http://hz.c1oappe.top/gtryfcfcgf.html

[U30] Py：数据类
来源：http://hz.ehwqpu.com/gtewnzrayi.html

@dataclass(slots=True)
来源：http://hz.zycfv.cn/gtjmzhjigi.html

[U31] Py：单测
来源：http://hz.shanyushiyangkeji.top/gtpwzgkqol.html

python -m pytest -q
来源：http://hz.yj20258.top/gtgxivcoev.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtkhlzmegh.html

ruff format . && ruff check --fix .
来源：http://hz.xuetiantiany.cn/gtqxcwyocn.html

[U33] Py：打包发布
来源：http://hz.yuxming.cn/gttqwtiaza.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gtjjvgcppz.html

[U34] Py：判断编码
来源：http://hz.aibaodan.cn/gttjcwqphq.html

chardet.detect(raw)
来源：http://hz.hfpthk.cn/gtsrjqjuvz.html

[U35] Py：发送邮件
来源：http://hz.birdmap.top/gtzmiizmnj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tianlin.xyz/gtynlqxdll.html

[U36] Py：定时任务
来源：http://hz.chenlongwang.top/gtdycgbzbv.html

schedule.every(10).minutes.do(job)
来源：http://hz.ybcxt.top/gtygetrsua.html

[U37] Py：读写 Excel
来源：http://hz.daxiang520.top/gtioujiikc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhijiandao.cn/gthhvnzcnx.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtdxrczhts.html

Path(__file__).resolve().parent
来源：http://hz.cashguo.top/gtxykvslcv.html

[U39] Py：判断是否在交互环境
来源：http://hz.pycfn.com/gtbtpswtqk.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtsrrzdtpc.html

[U40] Py：打印到标准错误
来源：http://hz.nanxinkj.top/gtrqfkdwkw.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtvdqqnsqc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinghuilouyu.cn/gtfskzueyr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xinyue.icu/gtusjuzkue.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtaoiuzwgf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhijiandao.cn/gtyzvhxfil.html

[U43] PHP：声明命名空间
来源：http://hz.birdmap.top/gtwarhrfew.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtmyuppugo.html

[U44] PHP：开启严格类型
来源：http://hz.gogol.net.cn/gttumjrogv.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtmmhhygew.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tian-w.cn/gtzjiloduu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtyetdxpnh.html

[U46] PHP：可空类型
来源：http://hz.shzxlz.cn/gtbdgooloa.html

?string $name = null
来源：http://hz.cucudq.cn/gtwbbtteun.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtyxsowkpv.html

int|string $id
来源：http://hz.andypj.xyz/gtpuasgzfc.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangkeji.top/gtbwyamcqg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daria6918.cn/gtqazzmiys.html

[U49] PHP：只读属性
来源：http://hz.jlsjyb.cn/gtxuvyliqf.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtwnufecjo.html

[U50] PHP：构造器属性提升
来源：http://hz.ybcxt.top/gtkxljripd.html

public function __construct(private int $id) {}
来源：http://hz.zdqjudy.top/gtpbojsbjl.html

[U51] PHP：数组解构
来源：http://hz.pengpengdd.cyou/gtuognfmmw.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtbyumvvnb.html

[U52] PHP：箭头函数
来源：http://hz.ywan-chungtsiang.top/gtidcforbo.html

$double = fn($x) => $x * 2;
来源：http://hz.cqqwz.cn/gtkkteyzci.html

[U53] PHP：空合并运算符
来源：http://hz.yonumen.top/gtfqtwvvxt.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258.top/gtmbqkstyq.html

[U54] PHP：空安全调用
来源：http://hz.chenjidiqi.icu/gtoxoxfkst.html

$obj?->method()
来源：http://hz.ybcxt.top/gtcqhvttzm.html

[U55] PHP：match 表达式
来源：http://hz.dianchejie.cn/gtpldoxner.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gtpxfnsmto.html

[U56] PHP：命名参数
来源：http://hz.pycfn.com/gtlklkzwvh.html

f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtxlufigfj.html

[U57] PHP：字符串插值
来源：http://hz.jinghuilouyu.cn/gtstwgrcbl.html

"值: {$a}"
来源：http://hz.hongshengwenyu.top/gtxlogdfbu.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtwwohfnct.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sxryk.cn/gtwghxevyu.html

[U59] PHP：自定义排序
来源：http://hz.tianlin.xyz/gtmbxdrlbk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtdmhzrzas.html

[U60] PHP：JSON 编解码
来源：http://hz.tanke756.top/gtanhrclkw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.redwolf501.top/gtynywchsu.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtnciklblr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gttdnywymt.html

[U62] PHP：日期对象
来源：http://hz.yueranfly.top/gtshsvlfua.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtlztmicct.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangkeji.top/gtcqhfuxxx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jyoumei.cn/gteimpbvcu.html

[U64] PHP：目录遍历
来源：http://hz.meibo888.top/gteibmljbp.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydjk.org.cn/gthxzkkxvm.html

[U65] PHP：会话
来源：http://hz.yuxming.cn/gttlfhthpc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tianlin.xyz/gtgcsuxrsb.html

[U66] PHP：设置 Cookie
来源：http://hz.kuanghao11.cn/gtzzpchhqi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gtnnvqmpeb.html

[U67] PHP：处理文件上传
来源：http://hz.yj202588.top/gtgygthfzf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.haohaochexian.top/gtccmayczc.html

[U68] PHP：PDO 连接
来源：http://hz.andypj.xyz/gtmjqdixey.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxinkj.top/gtoeycdppv.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gtiixtojim.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.fzhhl.top/gtgqghbkfp.html

[U70] PHP：PDO 事务
来源：http://hz.cashguo.top/gteihlvlxf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jlsjyb.cn/gtpywxtpsp.html

[U71] PHP：抛出异常
来源：http://hz.chenzaomai.com/gtflojdojm.html

throw new RuntimeException("失败", 500);
来源：http://hz.birdmap.top/gtkoqgtusw.html

[U72] PHP：写错误日志
来源：http://hz.tianlin.xyz/gtbkzfjynk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ppjwa.cn/gtgmsagkhh.html

[U73] PHP：读取 ini 配置
来源：http://hz.sufxvd.cn/gtzlzcufuo.html

parse_ini_file("config.ini", true)
来源：http://hz.nwbrower.top/gtazmizmdh.html

[U74] PHP：读取环境变量
来源：http://hz.jinqigfzy.top/gtvdpxuiuf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hywenlv.cn/gtdfcjapxf.html

[U75] PHP：依赖注入
来源：http://hz.pycfn.com/gtdgohjrmc.html

composer require psr/container
来源：http://hz.shuidangran.top/gtbwvekpyd.html

[U76] PHP：简单路由
来源：http://hz.gotoacloud.top/gtjyjxtlyz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.gaohongyu789.top/gthzhhfzcp.html

[U77] PHP：模板渲染
来源：http://hz.yuxming.cn/gtjlcquclg.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtdzwvutcp.html

[U78] PHP：单元测试
来源：http://hz.jqgufenzy.top/gtqkjxjvwq.html

composer require --dev phpunit/phpunit
来源：http://hz.zhoulong.xyz/gthdlgawdc.html

[U79] PHP：静态分析
来源：http://hz.fzhhl.top/gtdbizjdzq.html

composer require --dev phpstan/phpstan
来源：http://hz.pycfn.com/gtinftautu.html

[U80] PHP：代码规范修复
来源：http://hz.sxryk.cn/gtrwmagszf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtuekzyjqy.html

[U81] JS：初始化项目
来源：http://hz.chenzaomai.com/gttrmdbmwr.html

npm init -y;  npm i express
来源：http://hz.iojbl.cn/gtnrlxbfsq.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtonvwxdwd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shanyushiyangkeji.top/gtrjdijpvl.html

[U83] JS：ES Module 导入导出
来源：http://hz.gaohongyu789.top/gterjgqdde.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtstvwoewy.html

[U84] JS：CommonJS 写法
来源：http://hz.sufxvd.cn/gttbsfzram.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yonumen.top/gtsvckpdeb.html

[U85] JS：可选链
来源：http://hz.zhiwuduotai.top/gtlugdiivu.html

a?.b?.c
来源：http://hz.xuanzx.com/gtqaqwzvnz.html

[U86] JS：空值合并
来源：http://hz.andypj.xyz/gtutuipzzq.html

a ?? b
来源：http://hz.jyoumei.cn/gtqlcbmmlf.html

[U87] JS：解构默认值
来源：http://hz.yanxiufei.cn/gtfgnrhfui.html

const { a = 1, b = 2 } = obj;
来源：http://hz.guannengcc.top/gtiiqvmxlg.html

[U88] JS：对象展开合并
来源：http://hz.gotoacloud.top/gtkgfywevf.html

{ ...a, ...b }
来源：http://hz.wangdashe.top/gtkachfmxh.html

[U89] JS：数组去重
来源：http://hz.jinyuanbaomall.cn/gtmdhccsjd.html

[...new Set(arr)]
来源：http://hz.jianghu66.top/gtoyimxdxt.html

[U90] JS：数字数组排序
来源：http://hz.cheryme.top/gtwpbdsgul.html

[...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gttslnzvvn.html

[U91] JS：对象键值遍历
来源：http://hz.svipenyu.cn/gtontkodts.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.yuxming.cn/gtdggfesos.html

[U92] JS：深拷贝
来源：http://hz.shuidangran.top/gtcbrzupdt.html

structuredClone(obj)
来源：http://hz.aizwys.cn/gtjzpodyxv.html

[U93] JS：模板字符串
来源：http://hz.316326.xyz/gtfaupivph.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtxgolqemr.html

[U94] JS：箭头函数
来源：http://hz.fengsongda.top/gtdgqdtzep.html

const double = x => x * 2;
来源：http://hz.ppjwa.cn/gtnebbfewd.html

[U95] JS：Promise 包装
来源：http://hz.yonumen.top/gtpbuweobs.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtauudqmlu.html

[U96] JS：async/await 与异常
来源：http://hz.haohaochexian.top/gthnquugls.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtgvterauc.html

[U97] JS：并发请求
来源：http://hz.sxryk.cn/gtgvfyqewg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtzpjzhulb.html

[U98] JS：fetch 带 JSON
来源：http://hz.ydjk.org.cn/gtlhektorv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nanxinkj.top/gtbutmmcqe.html

[U99] JS：事件监听
来源：http://hz.sufxvd.cn/gtwwdhqndg.html

el.addEventListener("click", e => {})
来源：http://hz.zhijiandao.cn/gtnucfbgnl.html

[U100] JS：DOM 查询
来源：http://hz.shanyushiyangtech.top/gtpiqrkrnd.html

document.querySelector(".item")
来源：http://hz.tian-w.cn/gtiietbczk.html

[U101] JS：classList 操作
来源：http://hz.dianchejie.cn/gthsxilefj.html

el.classList.toggle("active")
来源：http://hz.nanxinkj.top/gtcntmgano.html

[U102] JS：本地存储
来源：http://hz.hnqzz.top/gtctowldql.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yuanzhike.top/gtynzqxljz.html

[U103] JS：定时器
来源：http://hz.dianchejie.cn/gtxvmuopjb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yvedp.cn/gtudahhzrf.html

[U104] JS：防抖
来源：http://hz.yuanzhike.top/gtrjlerlly.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtggeiwjse.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtcmlzcgdx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ppjwa.cn/gtngfxmyyj.html

[U106] JS：日期格式化
来源：http://hz.smart0.xyz/gtzfojrhms.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.gzhubu.top/gtygkxxstb.html

[U107] JS：数字千分位
来源：http://hz.sufxvd.cn/gtanbihplo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.redwolf501.top/gtbtfzssih.html

[U108] JS：随机整数
来源：http://hz.shzxlz.cn/gtcgnckdrv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.xylfe.cn/gtoxxujwou.html

[U109] JS：数组分组
来源：http://hz.zhengqikj.top/gthzaipica.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtcxialnqt.html

[U110] JS：数组分块
来源：http://hz.sweek.top/gtjyywlegx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.snrcjt.cn/gtlyyiesdh.html

[U111] JS：对象转 Map
来源：http://hz.tianlin.xyz/gtowufxidz.html

new Map(Object.entries(obj))
来源：http://hz.jinqigufen.top/gtfqcwuqeb.html

[U112] JS：字符串补位
来源：http://hz.nanxuanxn.top/gtaridreqs.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtlnapyeuj.html

[U113] JS：正则替换全部
来源：http://hz.ehwqpu.com/gtukdolefd.html

s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtsfnldzaz.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtnziikjcy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtvurvxclz.html

[U115] JS：生成 UUID
来源：http://hz.zhixingplan.top/gtgwtzbiof.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtlpwnhwnp.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gaohongyu789.top/gtcgdbwgmt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.jyoumei.cn/gtlefracob.html

[U117] JS：单元测试
来源：http://hz.zhoulong.xyz/gtsyqxzqfm.html

npm i -D vitest;  npx vitest
来源：http://hz.zdqjudy.top/gtqgnhwboa.html

[U118] JS：开发服务器
来源：http://hz.yuanzhike.top/gtjwisslbq.html

npm i -D vite;  npx vite
来源：http://hz.xziqi.cn/gtnhxnqdun.html

[U119] JS：生产构建
来源：http://hz.yuanzhike.top/gtyttzzstk.html

npx vite build
来源：http://hz.xingfuxueyuan.xyz/gtdvbbuxoj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.tian-w.cn/gtthwtfrdi.html

import.meta.env.VITE_API_URL
来源：http://hz.hysaishi.cn/gtqyjzanvm.html

================================================================================
来源：http://hz.gzhubu.top/gtvfismkvt.html

统计汇总
来源：http://hz.guannengcc.top/gtyscwpven.html

================================================================================
来源：http://hz.meibo888.top/gtkiivmzdv.html

按语言统计（条）：
来源：http://hz.cdnleiting.top/gtobxdhegn.html

Python ......... 252
来源：http://hz.jyoumei.cn/gtcanseugr.html

PHP ............ 252
来源：http://hz.xuanzx.com/gtxuqibqlb.html

JavaScript ..... 252
来源：http://hz.yangfankeji.com/gtpnxftsez.html

TypeScript ..... 212
来源：http://hz.nanxinkj.top/gtkortvwgi.html

Java ........... 212
来源：http://hz.cucudq.cn/gtenywqimi.html

Go ............. 212
来源：http://hz.ydzc1.top/gtbgxgkrrf.html

Ruby ........... 212
来源：http://hz.ppjwa.cn/gtirvhmkys.html

C# ............. 212
来源：http://hz.jqgfzy.top/gtcrkhuyyf.html

C .............. 30
来源：http://hz.ybcxt.top/gtrteyzlxd.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtpzcnnmvz.html

SQL ............ 90
来源：http://hz.gotoacloud.top/gtmzrihyjp.html

Bash ........... 80
来源：http://hz.yuanzhike.top/gtpjwtuqqq.html

Kotlin ......... 15
来源：http://hz.smart0.xyz/gtjiggvuoa.html

Swift .......... 15
来源：http://hz.xylfe.cn/gtdamcztaz.html

Lua ............ 10
来源：http://hz.cqqwz.cn/gtytfliqqu.html

Perl ........... 10
来源：http://hz.ybcxt.top/gtcfbzanzk.html

Scala .......... 10
来源：http://hz.birdmap.top/gtvlfdnnkq.html

------------------------------------
来源：http://hz.aibaodan.cn/gtnqhrltzy.html

合计 ........... 2106 条
来源：http://hz.jinyuanbaomall.cn/gtlyyyhnuc.html

按章节统计：
来源：http://hz.zhijiandao.cn/gtyornsgsq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gteggtfxxa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gttbqzrbbc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gttscydgfr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shangyingyoupin.top/gtmtuifoty.html


<!-- 参考信息 -->