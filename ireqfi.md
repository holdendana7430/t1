代发 wailian999

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtnuhedngl.html

for my $x (@arr) { print $x; }
来源：http://hz.daria6918.cn/gtwvdndxgb.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtstaljqno.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtktedxqod.html

[T47] Perl：正则捕获
来源：http://hz.shuidangran.top/gtpnyteguw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtlfmuwizz.html

[T48] Perl：正则替换
来源：http://hz.zhongyouzk.top/gtvaamewxx.html

$s =~ s/old/new/g;
来源：http://hz.yvedp.cn/gtrszdkahy.html

[T49] Perl：函数
来源：http://hz.xylfe.cn/gtbkxenzgz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenlongwang.top/gtbzfzjemi.html

[T50] Perl：逐行读文件
来源：http://hz.jlsjyb.cn/gtansyesox.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.0kj1m.cn/gtwkemwokx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gthooxshxu.html

[T51] Scala：Hello World
来源：http://hz.zhijiandao.cn/gtpuwsxkqh.html

println("Hello")
来源：http://hz.hnqzz.top/gtaoigzraq.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtwssdolxi.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtkwexojrf.html

[T53] Scala：字符串插值
来源：http://hz.zhongyouzk.top/gtvltfgnwo.html

s"值: $b"
来源：http://hz.9152youxi.cn/gtaeyuknmq.html

[T54] Scala：集合映射
来源：http://hz.gogol.net.cn/gtclppgbqs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cdnleiting.top/gtldixthbr.html

[T55] Scala：集合过滤
来源：http://hz.sweek.top/gtvmudboov.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtwyeqwgaa.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtxhfnnrma.html

case class User(name: String, age: Int)
来源：http://hz.0kj1m.cn/gttzmbcqiw.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtnwgkerij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258888.top/gtpntqfrxg.html

[T58] Scala：函数定义
来源：http://hz.jiagoushi.top/gtwjedvjoa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtkgfbiopf.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtafcdprql.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhiwuduotai.top/gtxcxondcg.html

[T60] Scala：折叠
来源：http://hz.316326.xyz/gtbhdkuuah.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtegbfpnhb.html

================================================================================
来源：http://hz.yonumen.top/gtuouginvj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtvixnvsxf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtycvmdekm.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtvtingrtz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangkeji.top/gtyzqrphsy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cqqwz.cn/gtwvyheaca.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guannengcc.top/gtxdshdxfn.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gtrjohwenx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj20258888.top/gtlarqrmtr.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gtycfosadt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cashguo.top/gtymykynbj.html

[U05] Py：列表去重且保序
来源：http://hz.sxryk.cn/gtlmgnrqqr.html

list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtcpgndbab.html

[U06] Py：合并两个字典
来源：http://hz.yj202588.top/gtkuvzdapz.html

{**a, **b}
来源：http://hz.zhixingplan.top/gtxcohwbem.html

[U07] Py：反转字典键值
来源：http://hz.pycfn.com/gttnqvhoon.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtaudahbjy.html

[U08] Py：展平二维列表
来源：http://hz.hysaishi.cn/gtcjfyykvg.html

[y for x in nested for y in x]
来源：http://hz.daria6918.cn/gtnyaidrta.html

[U09] Py：字典取最大值的键
来源：http://hz.jinyuanbaomall.cn/gthudnwron.html

max(d, key=d.get)
来源：http://hz.jlsjyb.cn/gtqqxrkyoq.html

[U10] Py：按值排序字典
来源：http://hz.iojbl.cn/gtwcwcqois.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxinkj.top/gtbymtcevb.html

[U11] Py：生成器表达式
来源：http://hz.tanke756.top/gtfrfrrcaz.html

(x * 2 for x in arr)
来源：http://hz.zhiwuduotai.top/gtiizrlkay.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtzeobnccq.html

Counter(arr).most_common(3)
来源：http://hz.cashguo.top/gtsmspisgf.html

[U13] Py：固定长度队列
来源：http://hz.hfpthk.cn/gtqapxdigv.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtjkhqztlv.html

[U14] Py：分组收集到列表
来源：http://hz.chenzaomai.com/gttsrpotwf.html

defaultdict(list)
来源：http://hz.cashguo.top/gtkeepqjzu.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gtnhcdimaq.html

t = time.perf_counter()
来源：http://hz.hywenlv.cn/gtetkavprr.html

[U16] Py：命令行参数解析
来源：http://hz.hfpthk.cn/gtkjxkkwzi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sysykeji.top/gtogxscyad.html

[U17] Py：初始化日志
来源：http://hz.ivvv.top/gtdrubhgqb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhoulong.xyz/gtktzmzoya.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtlrdttjlz.html

pat = re.compile(r"\d+")
来源：http://hz.ywan-chungtsiang.top/gtlfknjshp.html

[U19] Py：正则替换带回调
来源：http://hz.c1oappe.top/gtmjtsgmvr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtrdqxvxxb.html

[U20] Py：缓存函数结果
来源：http://hz.sufxvd.cn/gtfnceocew.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtaydldjlq.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhengqikj.top/gttijdelbj.html

@contextlib.contextmanager
来源：http://hz.cucudq.cn/gtuspmrzbd.html

[U22] Py：矩阵转置
来源：http://hz.pycfn.com/gtqiiribnq.html

list(zip(*m))
来源：http://hz.52xcode.cn/gtrylfians.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gtcdkhewjk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.aizwys.cn/gtifiiyybk.html

[U24] Py：路径操作
来源：http://hz.zycfv.cn/gtcjtmgzhq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.quarkkingdee.top/gtjcfcslzn.html

[U25] Py：CSV 按字典读
来源：http://hz.chenjidiqi.icu/gtsedraukg.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gthamqhrbm.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtcgqyfpxz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gtpujsuuxs.html

[U27] Py：异步 HTTP
来源：http://hz.xuetiantiany.cn/gttbxtakvl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jlsjyb.cn/gtpbvcrose.html

[U28] Py：类型别名
来源：http://hz.smart0.xyz/gtzvvdxkgq.html

UserId = int
来源：http://hz.jqgufenzy.top/gtodxaniix.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtjildttbk.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gtfpyydexl.html

[U30] Py：数据类
来源：http://hz.ywan-chungtsiang.top/gtqdpwywdh.html

@dataclass(slots=True)
来源：http://hz.ppjwa.cn/gtibhhtmkv.html

[U31] Py：单测
来源：http://hz.birdmap.top/gtitehyfwb.html

python -m pytest -q
来源：http://hz.jinqigufen.top/gtmbflwmuv.html

[U32] Py：代码格式化
来源：http://hz.zhixingplan.top/gtombaxtsm.html

ruff format . && ruff check --fix .
来源：http://hz.birdmap.top/gtmmkersuu.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtlkioyxcq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guannengcc.top/gttksguihl.html

[U34] Py：判断编码
来源：http://hz.chenlongwang.top/gtkxfsovun.html

chardet.detect(raw)
来源：http://hz.52xcode.cn/gtdcjakepi.html

[U35] Py：发送邮件
来源：http://hz.yuanzhike.top/gtmzpeflyl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yvedp.cn/gtvnhoksst.html

[U36] Py：定时任务
来源：http://hz.zhiwuduotai.top/gtjksugxel.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtzitlqkid.html

[U37] Py：读写 Excel
来源：http://hz.0kj1m.cn/gtumaibbca.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.birdmap.top/gtxgaflffv.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gtmvazudhb.html

Path(__file__).resolve().parent
来源：http://hz.ppjwa.cn/gtfbrakzze.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gtfmzlexcg.html

sys.stdout.isatty()
来源：http://hz.hysaishi.cn/gtgzjqabas.html

[U40] Py：打印到标准错误
来源：http://hz.xylfe.cn/gtzdvuezxq.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtjrulmedu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangdashe.top/gtvaipumvq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtorrmkecn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangkeji.top/gtnejbynss.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dianchejie.cn/gtgeopcden.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtvrpugcgx.html

namespace App\Http;
来源：http://hz.ydjk.org.cn/gthkziysip.html

[U44] PHP：开启严格类型
来源：http://hz.xziqi.cn/gttzmuykpo.html

declare(strict_types=1);
来源：http://hz.hongshengwenyu.top/gtxqaybtaz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtkmtxdhaq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtlnaxenlp.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtlfqkaybd.html

?string $name = null
来源：http://hz.wangshuangyany.cn/gtajowgsss.html

[U47] PHP：联合类型
来源：http://hz.xylfe.cn/gtiluamosw.html

int|string $id
来源：http://hz.jqgfzy.top/gtwmwwtkvh.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtijcdoklc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenlongwang.top/gtyzpmxlfl.html

[U49] PHP：只读属性
来源：http://hz.gotoacloud.top/gtvrzbdxah.html

public readonly string $name
来源：http://hz.daria6918.cn/gtnjidqdjx.html

[U50] PHP：构造器属性提升
来源：http://hz.yueranfly.top/gtmglvoihz.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtybnmlhah.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtxsewnlvl.html

[$a, $b] = $arr;
来源：http://hz.hysaishi.cn/gtlgrblfcx.html

[U52] PHP：箭头函数
来源：http://hz.shzxlz.cn/gtquiunakx.html

$double = fn($x) => $x * 2;
来源：http://hz.daxiang520.top/gtxcudoswi.html

[U53] PHP：空合并运算符
来源：http://hz.hnxiangtu.top/gthedydzvf.html

$v = $a ?? $b ?? "default";
来源：http://hz.nwbrower.top/gtlsgmhlht.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtdnwsohlb.html

$obj?->method()
来源：http://hz.zhengqikj.top/gtynekfoyu.html

[U55] PHP：match 表达式
来源：http://hz.fzhhl.top/gtvjidapxx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aibaodan.cn/gtmfundzsy.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtcghjepxh.html

f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtlnuinecv.html

[U57] PHP：字符串插值
来源：http://hz.zhixingplan.top/gtopsicjxe.html

"值: {$a}"
来源：http://hz.ydjk.org.cn/gtlfphhkkv.html

[U58] PHP：数组三件套
来源：http://hz.fzhhl.top/gtyehzbpty.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ppjwa.cn/gtmymlbvuz.html

[U59] PHP：自定义排序
来源：http://hz.cucudq.cn/gtdyqfetgo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtdgxrohxa.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangtech.top/gtnuroubjd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hysaishi.cn/gtcositavm.html

[U61] PHP：正则
来源：http://hz.zhijiandao.cn/gtnwvdihfd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtqytxayhq.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtoiyuolxb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.daria6918.cn/gtdyeagqil.html

[U63] PHP：文件读写
来源：http://hz.ivvv.top/gtjqrzdfkt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gzhubu.top/gtpkivbkfo.html

[U64] PHP：目录遍历
来源：http://hz.shzxlz.cn/gtyoxrlewx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.quarkkingdee.top/gtudktfgjt.html

[U65] PHP：会话
来源：http://hz.vqdsnc.cn/gtkfnsunbn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.havefunace.top/gtspcuoibw.html

[U66] PHP：设置 Cookie
来源：http://hz.snrcjt.cn/gtqpagufql.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yanxiufei.cn/gtxvfrccvu.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtjfqfkbqx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jinyuanbaomall.cn/gtswogdgsq.html

[U68] PHP：PDO 连接
来源：http://hz.xuanzx.com/gtolzorcbc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangkeji.top/gtacglwudx.html

[U69] PHP：PDO 预处理
来源：http://hz.yuanzhike.top/gtyvtyhwrq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shangyingyoupin.top/gtsrzcjmsl.html

[U70] PHP：PDO 事务
来源：http://hz.daria6918.cn/gtfakiageu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pengpengdd.cyou/gtnzmwarjm.html

[U71] PHP：抛出异常
来源：http://hz.shangyingyoupin.top/gtbpkmnlfl.html

throw new RuntimeException("失败", 500);
来源：http://hz.mhx1999.top/gtfikcmfzy.html

[U72] PHP：写错误日志
来源：http://hz.tianlin.xyz/gtfntrzurj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shzxlz.cn/gtlrgokuds.html

[U73] PHP：读取 ini 配置
来源：http://hz.kuanghao11.cn/gttqcudqkz.html

parse_ini_file("config.ini", true)
来源：http://hz.zhixingplan.top/gtstwrwxvb.html

[U74] PHP：读取环境变量
来源：http://hz.hnxiangtu.top/gtseqqjyje.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zycfv.cn/gtxowfilgq.html

[U75] PHP：依赖注入
来源：http://hz.hnxiangtu.top/gtatwrmzov.html

composer require psr/container
来源：http://hz.zhoulong.xyz/gtrkclwedp.html

[U76] PHP：简单路由
来源：http://hz.jinqigufen.top/gtuugdzruk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.fzhhl.top/gtlfeuybar.html

[U77] PHP：模板渲染
来源：http://hz.cheryme.top/gttseolqsz.html

composer require twig/twig
来源：http://hz.yangfankeji.com/gtsrvojqvy.html

[U78] PHP：单元测试
来源：http://hz.meibo888.top/gtfiejcpin.html

composer require --dev phpunit/phpunit
来源：http://hz.9152youxi.cn/gtpobteynp.html

[U79] PHP：静态分析
来源：http://hz.zhiwuduotai.top/gtxsrrubtp.html

composer require --dev phpstan/phpstan
来源：http://hz.xylfe.cn/gthpijzwys.html

[U80] PHP：代码规范修复
来源：http://hz.hammf.cn/gtlhkkjzdc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jqgufenzy.top/gtriktqjpg.html

[U81] JS：初始化项目
来源：http://hz.vqdsnc.cn/gtxulergzk.html

npm init -y;  npm i express
来源：http://hz.zhijiandao.cn/gtbzapbcds.html

[U82] JS：package.json 脚本
来源：http://hz.chenjidiqi.icu/gtbdojsgaw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.guannengcc.top/gtprnipocf.html

[U83] JS：ES Module 导入导出
来源：http://hz.shuidangran.top/gthtsigtml.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.chenjidiqi.icu/gtkylriqhr.html

[U84] JS：CommonJS 写法
来源：http://hz.smart0.xyz/gtccyqkqga.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.bjfxy.top/gtgkuhkmpo.html

[U85] JS：可选链
来源：http://hz.smart0.xyz/gtgtvhwowm.html

a?.b?.c
来源：http://hz.shanyushiyangtech.top/gthstpzvfk.html

[U86] JS：空值合并
来源：http://hz.cucudq.cn/gtifdmoecn.html

a ?? b
来源：http://hz.aizwys.cn/gtsinynbpo.html

[U87] JS：解构默认值
来源：http://hz.birdmap.top/gthzqmymik.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhiwuduotai.top/gtbfgxfhwi.html

[U88] JS：对象展开合并
来源：http://hz.gzhubu.top/gtbmiwhjtf.html

{ ...a, ...b }
来源：http://hz.yongpay.top/gtkqnzrujr.html

[U89] JS：数组去重
来源：http://hz.wangdashe.top/gtfbzjihjk.html

[...new Set(arr)]
来源：http://hz.sweek.top/gttpwcqxxx.html

[U90] JS：数字数组排序
来源：http://hz.gzhubu.top/gtpfrrppav.html

[...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtqvzklteu.html

[U91] JS：对象键值遍历
来源：http://hz.wangshuangyany.cn/gtpcwxbqsd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtqnhvhmlv.html

[U92] JS：深拷贝
来源：http://hz.chenjidiqi.icu/gtpqmuehkk.html

structuredClone(obj)
来源：http://hz.sysykeji.top/gtimkvxtpf.html

[U93] JS：模板字符串
来源：http://hz.zhiwuduotai.top/gtyzmfjdus.html

`共 ${n} 条`
来源：http://hz.shanyushiyangkeji.top/gtkrvilnhj.html

[U94] JS：箭头函数
来源：http://hz.xinyue.icu/gtqtuzbfgt.html

const double = x => x * 2;
来源：http://hz.bjfxy.top/gtukjvrkqf.html

[U95] JS：Promise 包装
来源：http://hz.c1oappe.top/gtlhccxlld.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtpehdwfvg.html

[U96] JS：async/await 与异常
来源：http://hz.cheryme.top/gteolsduwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtfrqrhlrj.html

[U97] JS：并发请求
来源：http://hz.yvedp.cn/gtrfzqchkv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtlpckaymm.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangshuangyany.cn/gtwpxqqguc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hammf.cn/gtgzeewilb.html

[U99] JS：事件监听
来源：http://hz.meibo888.top/gtpmdsgvaw.html

el.addEventListener("click", e => {})
来源：http://hz.xylfe.cn/gtrkkmzfgy.html

[U100] JS：DOM 查询
来源：http://hz.guowangkeji.top/gthspnghle.html

document.querySelector(".item")
来源：http://hz.guowangkeji.top/gtoclxnyjx.html

[U101] JS：classList 操作
来源：http://hz.fzhhl.top/gtrkxkzrjh.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtwrtyojkx.html

[U102] JS：本地存储
来源：http://hz.shzxlz.cn/gtnljrrndc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hywenlv.cn/gtgalvqlim.html

[U103] JS：定时器
来源：http://hz.ivvv.top/gtfzkyodta.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.dashuyun.cn/gtxturqcos.html

[U104] JS：防抖
来源：http://hz.xingfuxueyuan.xyz/gtuzjqxglp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtmesvthhl.html

[U105] JS：节流
来源：http://hz.snrcjt.cn/gtpywuzdmu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yueranfly.top/gtgfoabogl.html

[U106] JS：日期格式化
来源：http://hz.shanyushiyangkeji.top/gtwgkwrzqf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yongpay.top/gtgczmsinz.html

[U107] JS：数字千分位
来源：http://hz.shanyushiyangtech.top/gtcxiemehu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtafvisvfr.html

[U108] JS：随机整数
来源：http://hz.ywan-chungtsiang.top/gtqiqgvxtu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ywan-chungtsiang.top/gtonpjnhuf.html

[U109] JS：数组分组
来源：http://hz.pycfn.com/gtjjpstyjj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtqrxprffe.html

[U110] JS：数组分块
来源：http://hz.kuanghao11.cn/gtpfyobzch.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.nwbrower.top/gthplkacnh.html

[U111] JS：对象转 Map
来源：http://hz.pengpengdd.cyou/gttcjehsgk.html

new Map(Object.entries(obj))
来源：http://hz.nanxuanxn.top/gtngvgpory.html

[U112] JS：字符串补位
来源：http://hz.gaohongyu789.top/gtzlwoahdg.html

"7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtobiltbia.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtmmqncnnb.html

s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtqkfwggyb.html

[U114] JS：JSON 深比较
来源：http://hz.ivvv.top/gtjncyxlvl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.aibaodan.cn/gtexbcybet.html

[U115] JS：生成 UUID
来源：http://hz.yvedp.cn/gtxhaxxmdv.html

crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gtszmihysh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gotoacloud.top/gtbxejaqqs.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtvrbkyvih.html

[U117] JS：单元测试
来源：http://hz.hammf.cn/gtmejilrhm.html

npm i -D vitest;  npx vitest
来源：http://hz.xuetiantiany.cn/gtmpljilxp.html

[U118] JS：开发服务器
来源：http://hz.snrcjt.cn/gtmlrhzkcm.html

npm i -D vite;  npx vite
来源：http://hz.gzhubu.top/gtytpugxtx.html

[U119] JS：生产构建
来源：http://hz.sxryk.cn/gtjwcajlpv.html

npx vite build
来源：http://hz.zdqjudy.top/gtovcidxta.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.fzhhl.top/gtqmsscrvi.html

import.meta.env.VITE_API_URL
来源：http://hz.xinyue.icu/gtnlfeehuk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmgrgybhn.html

统计汇总
来源：http://hz.yuanzhike.top/gtbrtwydvt.html

================================================================================
来源：http://hz.tanke756.top/gtsciueavn.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtikykxlew.html

Python ......... 252
来源：http://hz.hfpthk.cn/gtyiepwhgf.html

PHP ............ 252
来源：http://hz.ehwqpu.com/gtbevvvgxn.html

JavaScript ..... 252
来源：http://hz.zhaomingkeji.xyz/gtjtuxysfi.html

TypeScript ..... 212
来源：http://hz.jiagoushi.top/gtqqnauzbo.html

Java ........... 212
来源：http://hz.andypj.xyz/gtvkpbkfcc.html

Go ............. 212
来源：http://hz.yvedp.cn/gtnegykvhf.html

Ruby ........... 212
来源：http://hz.xinyue.icu/gtxeqwdnrl.html

C# ............. 212
来源：http://hz.pengpengdd.cyou/gtzmviaejv.html

C .............. 30
来源：http://hz.xylfe.cn/gtawjnrzer.html

C++ ............ 30
来源：http://hz.haohaochexian.top/gtnupwofpm.html

SQL ............ 90
来源：http://hz.yuanzhike.top/gtvwvktbwz.html

Bash ........... 80
来源：http://hz.shanyushiyangtech.top/gtagkjwclq.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtrghwrrot.html

Swift .......... 15
来源：http://hz.shanyushiyangkeji.top/gtdynzmjba.html

Lua ............ 10
来源：http://hz.wangdashe.top/gttlgsqodp.html

Perl ........... 10
来源：http://hz.quarkkingdee.top/gtpulufsyd.html

Scala .......... 10
来源：http://hz.ehwqpu.com/gtqenywxdy.html

------------------------------------
来源：http://hz.xuetiantiany.cn/gtklrfaimq.html

合计 ........... 2106 条
来源：http://hz.nanxuanxn.top/gtxebdrjrk.html

按章节统计：
来源：http://hz.svipenyu.cn/gtpfhbmflz.html


<!-- 参考信息 -->