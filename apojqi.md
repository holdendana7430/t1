代发 wailian999

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtjtcycwcv.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtksucdlmw.html

[T46] Perl：哈希操作
来源：http://hz.sxryk.cn/gtebqqzymc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.smart0.xyz/gtislikjut.html

[T47] Perl：正则捕获
来源：http://hz.bjfxy.top/gtckrtplpb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.52xcode.cn/gtgbazvwnx.html

[T48] Perl：正则替换
来源：http://hz.zhaomingkeji.xyz/gtalendopp.html

$s =~ s/old/new/g;
来源：http://hz.c1oappe.top/gtsgasyzus.html

[T49] Perl：函数
来源：http://hz.jinqigufen.top/gtltfjeirp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gtvrvfabvm.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtkbinfpqf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtkstmsgqn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtdwfsxldq.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtftaajiop.html

println("Hello")
来源：http://hz.sxryk.cn/gtkyenippp.html

[T52] Scala：变量
来源：http://hz.shzxlz.cn/gtfeezfexe.html

val a = 1;  var b = 2
来源：http://hz.feifeiyinyue.top/gtnelvsshl.html

[T53] Scala：字符串插值
来源：http://hz.yangfankeji.com/gtihkczjda.html

s"值: $b"
来源：http://hz.cashguo.top/gttwnvgqxx.html

[T54] Scala：集合映射
来源：http://hz.smart0.xyz/gtnskuekww.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangkeji.top/gtvxnnwdfr.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gtbzxpkwvj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.haohaochexian.top/gtumdqgxtt.html

[T56] Scala：样例类
来源：http://hz.nanxuanxn.top/gttybwoeaf.html

case class User(name: String, age: Int)
来源：http://hz.yj20258.top/gtjonkeamh.html

[T57] Scala：模式匹配
来源：http://hz.svipenyu.cn/gtfbcchqyu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.smart0.xyz/gtmbvwssml.html

[T58] Scala：函数定义
来源：http://hz.xuanzx.com/gtadgcmkwo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydjk.org.cn/gteykafpzr.html

[T59] Scala：循环
来源：http://hz.nanxuanxn.top/gtpfvkpaiu.html

for (i <- 1 to 10) println(i)
来源：http://hz.fengsongda.top/gtlsdjeprd.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtjvebmbsq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aibaodan.cn/gtrptryayd.html

================================================================================
来源：http://hz.yvedp.cn/gtknuqisby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtrkmjykot.html

================================================================================
来源：http://hz.havefunace.top/gtujrxbxyo.html

[U01] Py：创建虚拟环境
来源：http://hz.daria6918.cn/gtourhelat.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtokjtrnbn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gtiamtrfmh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtzwbbzcwt.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gtbicepkdz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.wangdashe.top/gtrdrcdiwl.html

[U04] Py：变量调试打印
来源：http://hz.nwbrower.top/gtyrghezhs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hammf.cn/gtuwadbuml.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtqtsmzyjj.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtnvtxgxdj.html

[U06] Py：合并两个字典
来源：http://hz.iojbl.cn/gtzasgmfmw.html

{**a, **b}
来源：http://hz.hongshengwenyu.top/gthvjxbqmj.html

[U07] Py：反转字典键值
来源：http://hz.zhongyouzk.top/gtgbnyiapd.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtjgztwftf.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtnsllowgt.html

[y for x in nested for y in x]
来源：http://hz.xuetiantiany.cn/gtskmjfjyl.html

[U09] Py：字典取最大值的键
来源：http://hz.zhoulong.xyz/gtxglrrdzt.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtggillfbg.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gtkgpihkqb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gtwajohimx.html

[U11] Py：生成器表达式
来源：http://hz.svipenyu.cn/gttcqjgmnn.html

(x * 2 for x in arr)
来源：http://hz.hongshengwenyu.top/gtlxslfkko.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xziqi.cn/gtjkpjzwqd.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtyamsaztn.html

[U13] Py：固定长度队列
来源：http://hz.pengpengdd.cyou/gtutsiihtr.html

deque(maxlen=10)
来源：http://hz.zhixingplan.top/gtotaklstt.html

[U14] Py：分组收集到列表
来源：http://hz.xuanzx.com/gtbrlduutw.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtmvnzenvc.html

[U15] Py：高精度计时
来源：http://hz.ydjk.org.cn/gtdrsobnvv.html

t = time.perf_counter()
来源：http://hz.xylfe.cn/gtumnbabxq.html

[U16] Py：命令行参数解析
来源：http://hz.gaohongyu789.top/gtitcsdqzo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.redwolf501.top/gtaxgoakwo.html

[U17] Py：初始化日志
来源：http://hz.zhijiandao.cn/gtosujyxxi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtpimirdxz.html

[U18] Py：预编译正则
来源：http://hz.hongshengwenyu.top/gtfbpzjulf.html

pat = re.compile(r"\d+")
来源：http://hz.daria6918.cn/gtpormtrpf.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtztpbnvme.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ppjwa.cn/gtcqnwexcu.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtahlvqiis.html

@functools.lru_cache(maxsize=None)
来源：http://hz.haohaochexian.top/gtqfglsgbc.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangdashe.top/gturbhgxvl.html

@contextlib.contextmanager
来源：http://hz.jinqigfzy.top/gtenvuepbl.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtihxtpjya.html

list(zip(*m))
来源：http://hz.hywenlv.cn/gtvrbfctee.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gtrbjpafzy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangtech.top/gtzrjlemtu.html

[U24] Py：路径操作
来源：http://hz.jinqigfzy.top/gtlaxvrrpd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gthnxpuzxd.html

[U25] Py：CSV 按字典读
来源：http://hz.shanyushiyangtech.top/gtqtigfuqi.html

csv.DictReader(f)
来源：http://hz.hongshengwenyu.top/gtoculchug.html

[U26] Py：并发下载
来源：http://hz.svipenyu.cn/gtdbirgvbq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.0kj1m.cn/gtivsvunnq.html

[U27] Py：异步 HTTP
来源：http://hz.dashuyun.cn/gtrxeilqkx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtcleivnri.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtwvasular.html

UserId = int
来源：http://hz.fengsongda.top/gtqyvepzuv.html

[U29] Py：属性校验
来源：http://hz.daria6918.cn/gtvarxmxpf.html

@property 与 @x.setter 配合
来源：http://hz.nwbrower.top/gtytumczmv.html

[U30] Py：数据类
来源：http://hz.wangshuangyany.cn/gtdzveuztb.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtibjcckpt.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gtkprczvwb.html

python -m pytest -q
来源：http://hz.sufxvd.cn/gtutzzhenl.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangtech.top/gttxmhibsv.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtcctjazfo.html

[U33] Py：打包发布
来源：http://hz.xingfuxueyuan.xyz/gtnkawrssq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ywan-chungtsiang.top/gtkkmnufrj.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtfuuyyuoz.html

chardet.detect(raw)
来源：http://hz.meibo888.top/gtjohuiumg.html

[U35] Py：发送邮件
来源：http://hz.zhoulong.xyz/gtngeblxqa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gtjvmwokhf.html

[U36] Py：定时任务
来源：http://hz.ybcxt.top/gtymrqdgcm.html

schedule.every(10).minutes.do(job)
来源：http://hz.tianlin.xyz/gtnlscpdwc.html

[U37] Py：读写 Excel
来源：http://hz.sxryk.cn/gtowaxlbci.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.fzhhl.top/gttkhtwcpp.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gtksfedmef.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtcfjkyvqb.html

[U39] Py：判断是否在交互环境
来源：http://hz.ydzc1.top/gtehsrfksm.html

sys.stdout.isatty()
来源：http://hz.nanxuanxn.top/gtplmmbpyr.html

[U40] Py：打印到标准错误
来源：http://hz.daria6918.cn/gtsirdnstv.html

print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtpjrjqzmz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxinkj.top/gturvyllal.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ppjwa.cn/gttsfpcbnz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shangyingyoupin.top/gtlekrqybh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shuidangran.top/gtznxoxpwc.html

[U43] PHP：声明命名空间
来源：http://hz.c1oappe.top/gtetepagvm.html

namespace App\Http;
来源：http://hz.jqgufenzy.top/gtspkjaitx.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gthmzenmoz.html

declare(strict_types=1);
来源：http://hz.jianghu66.top/gtagfqdznx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dashuyun.cn/gtdlmhpfjn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtnpwxiscl.html

[U46] PHP：可空类型
来源：http://hz.tianlin.xyz/gtkgbzpaiq.html

?string $name = null
来源：http://hz.hnqzz.top/gtfoagerxe.html

[U47] PHP：联合类型
来源：http://hz.cqqwz.cn/gtgqakfbmx.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtbwrforph.html

[U48] PHP：纯枚举
来源：http://hz.mhx1999.top/gtljoevhpj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sweek.top/gtybdvifmk.html

[U49] PHP：只读属性
来源：http://hz.cqqwz.cn/gtbdhdrynb.html

public readonly string $name
来源：http://hz.tian-w.cn/gtwebkyjtt.html

[U50] PHP：构造器属性提升
来源：http://hz.feifeiyinyue.top/gtnjkrvqrt.html

public function __construct(private int $id) {}
来源：http://hz.jinyuanbaomall.cn/gtkkpzeweu.html

[U51] PHP：数组解构
来源：http://hz.gotoacloud.top/gtaajwuudw.html

[$a, $b] = $arr;
来源：http://hz.daria6918.cn/gtucedotvn.html

[U52] PHP：箭头函数
来源：http://hz.hongshengwenyu.top/gtltwolzgn.html

$double = fn($x) => $x * 2;
来源：http://hz.andypj.xyz/gtpwudglva.html

[U53] PHP：空合并运算符
来源：http://hz.aizwys.cn/gtmelekhth.html

$v = $a ?? $b ?? "default";
来源：http://hz.cucudq.cn/gtaioonfbw.html

[U54] PHP：空安全调用
来源：http://hz.yj20258.top/gtxctaafuj.html

$obj?->method()
来源：http://hz.jianghu66.top/gtumxjjtpx.html

[U55] PHP：match 表达式
来源：http://hz.zycfv.cn/gtshljlvhw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cashguo.top/gtgvphzfmx.html

[U56] PHP：命名参数
来源：http://hz.xziqi.cn/gtzfblpfjr.html

f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtvipoapci.html

[U57] PHP：字符串插值
来源：http://hz.jinghuilouyu.cn/gtqkhauiwh.html

"值: {$a}"
来源：http://hz.gzhubu.top/gtwmymmwio.html

[U58] PHP：数组三件套
来源：http://hz.iojbl.cn/gtbqzczobi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhixingplan.top/gtnrvvwtaf.html

[U59] PHP：自定义排序
来源：http://hz.zhaomingkeji.xyz/gtishilthe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hywenlv.cn/gtmtzwghmf.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtkkyqpirv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.bjfxy.top/gtmxhakiop.html

[U61] PHP：正则
来源：http://hz.52xcode.cn/gtftjgwxrg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtexjrmwqa.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gteryqzatj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtftjtgihk.html

[U63] PHP：文件读写
来源：http://hz.hysaishi.cn/gtavfdaeyj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.nanxinkj.top/gtbrzebwsw.html

[U64] PHP：目录遍历
来源：http://hz.dianchejie.cn/gtrknoxogf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtdywpgyme.html

[U65] PHP：会话
来源：http://hz.cashguo.top/gtqrrzcyst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.fengsongda.top/gtheqqkkuu.html

[U66] PHP：设置 Cookie
来源：http://hz.xingfuxueyuan.xyz/gtyowqyegi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtjsstkmap.html

[U67] PHP：处理文件上传
来源：http://hz.ppjwa.cn/gtbrmthvoe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hfpthk.cn/gtizckwjgm.html

[U68] PHP：PDO 连接
来源：http://hz.jinghuilouyu.cn/gtkaoehdaz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.kuanghao11.cn/gtzadkyora.html

[U69] PHP：PDO 预处理
来源：http://hz.zhengqikj.top/gtgpmvzdrk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shangyingyoupin.top/gtigwpmhnr.html

[U70] PHP：PDO 事务
来源：http://hz.zhengqikj.top/gtghqpgfev.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.316326.xyz/gtwgicaebe.html

[U71] PHP：抛出异常
来源：http://hz.yj20258888.top/gtjryryvso.html

throw new RuntimeException("失败", 500);
来源：http://hz.aibaodan.cn/gtmtwurvyo.html

[U72] PHP：写错误日志
来源：http://hz.zhijiandao.cn/gtlnpjecut.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinyuanbaomall.cn/gtakdxpjoz.html

[U73] PHP：读取 ini 配置
来源：http://hz.redwolf501.top/gtnifjvckp.html

parse_ini_file("config.ini", true)
来源：http://hz.feifeiyinyue.top/gtvlkasuji.html

[U74] PHP：读取环境变量
来源：http://hz.dashuyun.cn/gtcfxeoeic.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xinyue.icu/gtqglyllyr.html

[U75] PHP：依赖注入
来源：http://hz.jqgfzy.top/gtokzgcihj.html

composer require psr/container
来源：http://hz.smart0.xyz/gtiyzloggx.html

[U76] PHP：简单路由
来源：http://hz.chenlongwang.top/gtiqbygcxo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ydjk.org.cn/gtjxifcxoc.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtzgdlkhfl.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtujteyfvi.html

[U78] PHP：单元测试
来源：http://hz.cheryme.top/gtdtkuksmz.html

composer require --dev phpunit/phpunit
来源：http://hz.316326.xyz/gtnuaylmwp.html

[U79] PHP：静态分析
来源：http://hz.andypj.xyz/gtfjwaexcb.html

composer require --dev phpstan/phpstan
来源：http://hz.yuanzhike.top/gtgrfhifnx.html

[U80] PHP：代码规范修复
来源：http://hz.sweek.top/gtjayatrbv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yuanzhike.top/gtvurmmxmm.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtxonmaahq.html

npm init -y;  npm i express
来源：http://hz.shanyushiyangtech.top/gtupgjcxez.html

[U82] JS：package.json 脚本
来源：http://hz.jiagoushi.top/gtcuebsrie.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yangfankeji.com/gtspnhvtxx.html

[U83] JS：ES Module 导入导出
来源：http://hz.ydzc1.top/gtxjychxeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.nanxuanxn.top/gtcwipcsfs.html

[U84] JS：CommonJS 写法
来源：http://hz.hywenlv.cn/gtzaghyszi.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.havefunace.top/gtihsvysyj.html

[U85] JS：可选链
来源：http://hz.jinqigufen.top/gtmtzdbnst.html

a?.b?.c
来源：http://hz.cashguo.top/gtwxnrugrn.html

[U86] JS：空值合并
来源：http://hz.shanyushiyangkeji.top/gtkofznwbo.html

a ?? b
来源：http://hz.shangyingyoupin.top/gtrbfzbxlj.html

[U87] JS：解构默认值
来源：http://hz.52xcode.cn/gtteapqoxu.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yanxiufei.cn/gtdjykzvuf.html

[U88] JS：对象展开合并
来源：http://hz.cucudq.cn/gtjvzrssvn.html

{ ...a, ...b }
来源：http://hz.yvedp.cn/gtdshdzojz.html

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtosvybqmn.html

[...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtrwllzlft.html

[U90] JS：数字数组排序
来源：http://hz.cashguo.top/gtumjamrms.html

[...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtojuxnwcy.html

[U91] JS：对象键值遍历
来源：http://hz.andypj.xyz/gtuugadkoz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.snrcjt.cn/gtmxuttvig.html

[U92] JS：深拷贝
来源：http://hz.ydzc1.top/gtfthulaav.html

structuredClone(obj)
来源：http://hz.jiagoushi.top/gtknrkqmzg.html

[U93] JS：模板字符串
来源：http://hz.jinghuilouyu.cn/gtvqjvnfeq.html

`共 ${n} 条`
来源：http://hz.aibaodan.cn/gtrqbpchcu.html

[U94] JS：箭头函数
来源：http://hz.jiagoushi.top/gtjnioynps.html

const double = x => x * 2;
来源：http://hz.hongshengwenyu.top/gtehrlfgor.html

[U95] JS：Promise 包装
来源：http://hz.ywan-chungtsiang.top/gtbekrwkmd.html

new Promise((resolve, reject) => {})
来源：http://hz.ywan-chungtsiang.top/gtmrtrrxkw.html

[U96] JS：async/await 与异常
来源：http://hz.haohaochexian.top/gtgemymxfl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtouixvwst.html

[U97] JS：并发请求
来源：http://hz.zhixingplan.top/gtbxdyafyu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtxikgjxly.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtboqlbwlm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daxiang520.top/gthfgmcrvy.html

[U99] JS：事件监听
来源：http://hz.jlsjyb.cn/gtxaawiefw.html

el.addEventListener("click", e => {})
来源：http://hz.gogol.net.cn/gtcmqrzqkp.html

[U100] JS：DOM 查询
来源：http://hz.0kj1m.cn/gtzrqumrna.html

document.querySelector(".item")
来源：http://hz.jyoumei.cn/gtsewqrajv.html

[U101] JS：classList 操作
来源：http://hz.guannengcc.top/gtpvjjdrfj.html

el.classList.toggle("active")
来源：http://hz.zhoulong.xyz/gtxdxtqekq.html

[U102] JS：本地存储
来源：http://hz.quarkkingdee.top/gtqhzdkuvc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yangfankeji.com/gtnkaduftf.html

[U103] JS：定时器
来源：http://hz.smart0.xyz/gtdixzrdxs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shuidangran.top/gtkkthdfgl.html

[U104] JS：防抖
来源：http://hz.hammf.cn/gtmakjxdoj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtcwcwopdt.html

[U105] JS：节流
来源：http://hz.gotoacloud.top/gtidlvdwwk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hammf.cn/gtorbzbysy.html

[U106] JS：日期格式化
来源：http://hz.hongshengwenyu.top/gtzpuhneuh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yvedp.cn/gtahhbvjnf.html

[U107] JS：数字千分位
来源：http://hz.snrcjt.cn/gttulndnwr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.kuanghao11.cn/gttxfvhvbk.html

[U108] JS：随机整数
来源：http://hz.yueranfly.top/gtgcaugpwi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tianlin.xyz/gtiomausqr.html

[U109] JS：数组分组
来源：http://hz.vqdsnc.cn/gtieeamfpy.html

Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtazujzowa.html

[U110] JS：数组分块
来源：http://hz.yueranfly.top/gtkmhsxtrh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xuetiantiany.cn/gtanlhczun.html

[U111] JS：对象转 Map
来源：http://hz.tianlin.xyz/gtkzbfunjl.html

new Map(Object.entries(obj))
来源：http://hz.bjfxy.top/gtvrytwhpc.html

[U112] JS：字符串补位
来源：http://hz.yj20258.top/gtizfzgrio.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtmgldztxp.html

[U113] JS：正则替换全部
来源：http://hz.shuidangran.top/gthvmvydxg.html

s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtcmgsdwsn.html

[U114] JS：JSON 深比较
来源：http://hz.fengsongda.top/gtvitglcch.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtaecwvkvp.html

[U115] JS：生成 UUID
来源：http://hz.cqqwz.cn/gtkxgwvrlt.html

crypto.randomUUID()
来源：http://hz.cheryme.top/gtbomxhpmm.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigfzy.top/gtygdmqvud.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtarojtsev.html

[U117] JS：单元测试
来源：http://hz.ppjwa.cn/gtmtkoaeqc.html

npm i -D vitest;  npx vitest
来源：http://hz.aibaodan.cn/gtmdgwbjss.html

[U118] JS：开发服务器
来源：http://hz.haohaochexian.top/gtylnvaazu.html

npm i -D vite;  npx vite
来源：http://hz.chenjidiqi.icu/gtyblcywrf.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtggekpuzg.html

npx vite build
来源：http://hz.zhongyouzk.top/gtcczupzae.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhongyouzk.top/gttvsjlncw.html

import.meta.env.VITE_API_URL
来源：http://hz.gogol.net.cn/gtfhxrchwv.html

================================================================================
来源：http://hz.ivvv.top/gtudhnnpcu.html

统计汇总
来源：http://hz.hammf.cn/gtdjdgdwmc.html

================================================================================
来源：http://hz.zhengqikj.top/gtuubdwwpu.html

按语言统计（条）：
来源：http://hz.svipenyu.cn/gtwtodsswb.html

Python ......... 252
来源：http://hz.wangdashe.top/gtxaifixnu.html

PHP ............ 252
来源：http://hz.cqqwz.cn/gtnyheazta.html

JavaScript ..... 252
来源：http://hz.fzhhl.top/gtlrlkeqfd.html

TypeScript ..... 212
来源：http://hz.aibaodan.cn/gtjqzrzqjb.html

Java ........... 212
来源：http://hz.hysaishi.cn/gthoegwwjj.html

Go ............. 212
来源：http://hz.jiagoushi.top/gtczhzgwtk.html

Ruby ........... 212
来源：http://hz.haohaochexian.top/gtnheejyvu.html

C# ............. 212
来源：http://hz.shangyingyoupin.top/gtakcpzhym.html

C .............. 30
来源：http://hz.tanke756.top/gtarcyzown.html

C++ ............ 30
来源：http://hz.mhx1999.top/gtacnmkjvx.html

SQL ............ 90
来源：http://hz.xuetiantiany.cn/gtzjcvvjwv.html

Bash ........... 80
来源：http://hz.c1oappe.top/gtrnhpthpb.html

Kotlin ......... 15
来源：http://hz.ydjk.org.cn/gtxxkcocgq.html

Swift .......... 15
来源：http://hz.ydjk.org.cn/gtzyotxngx.html

Lua ............ 10
来源：http://hz.fzhhl.top/gtrwupifhq.html

Perl ........... 10
来源：http://hz.jianghu66.top/gtpbjxnhgx.html

Scala .......... 10
来源：http://hz.guannengcc.top/gtdvmtmbyh.html

------------------------------------
来源：http://hz.ppjwa.cn/gtneaqhspr.html

合计 ........... 2106 条
来源：http://hz.jianghu66.top/gtkqdyrsrf.html

按章节统计：
来源：http://hz.gotoacloud.top/gtpwrbhwek.html


<!-- 参考信息 -->