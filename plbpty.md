代发 wailian999

[T49] Perl：函数
来源：http://hz.sufxvd.cn/gtctehjibe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gtdeklkzln.html

[T50] Perl：逐行读文件
来源：http://hz.vqdsnc.cn/gtcszzoyxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtxmbyndvt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shzxlz.cn/gtznlylhlu.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtiiceztug.html

println("Hello")
来源：http://hz.sxryk.cn/gtxzvvzesz.html

[T52] Scala：变量
来源：http://hz.shuidangran.top/gtfimytvjg.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtphfweoqw.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtifqcxmae.html

s"值: $b"
来源：http://hz.yonumen.top/gtuktyltue.html

[T54] Scala：集合映射
来源：http://hz.hfpthk.cn/gttgidjctu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxuanxn.top/gtunhmmqyg.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtcwfuxbnr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cheryme.top/gtclneyfdb.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gtwndsfmym.html

case class User(name: String, age: Int)
来源：http://hz.redwolf501.top/gtyzaviuob.html

[T57] Scala：模式匹配
来源：http://hz.gotoacloud.top/gtiptzxfne.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dashuyun.cn/gtggxnewwb.html

[T58] Scala：函数定义
来源：http://hz.gzhubu.top/gtgkeekbek.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhijiandao.cn/gtcpotxrbw.html

[T59] Scala：循环
来源：http://hz.tanke756.top/gtyizjugeb.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj202588.top/gtjzgaicsl.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gthgjbtmli.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenzaomai.com/gtwyugjshx.html

================================================================================
来源：http://hz.chenlongwang.top/gtfqntmurk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tanke756.top/gtvwvudnpb.html

================================================================================
来源：http://hz.fengsongda.top/gtynjnonmg.html

[U01] Py：创建虚拟环境
来源：http://hz.yj202588.top/gtlfuvjanx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.52xcode.cn/gtorrwhswa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gtiiitspsw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydzc1.top/gtijdoqtml.html

[U03] Py：加载 .env 配置
来源：http://hz.9152youxi.cn/gtqrirhawg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtzytqvwzs.html

[U04] Py：变量调试打印
来源：http://hz.haohaochexian.top/gtrbydjlya.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtirpxbsmo.html

[U05] Py：列表去重且保序
来源：http://hz.mhx1999.top/gtmxznrwdp.html

list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtueyhuiuq.html

[U06] Py：合并两个字典
来源：http://hz.pycfn.com/gtplkeqans.html

{**a, **b}
来源：http://hz.yj20258888.top/gtnauibztf.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gtxftdwqnq.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtcgmcyyji.html

[U08] Py：展平二维列表
来源：http://hz.chenjidiqi.icu/gtkgkeefwg.html

[y for x in nested for y in x]
来源：http://hz.ydzc1.top/gtoifymhsq.html

[U09] Py：字典取最大值的键
来源：http://hz.nwbrower.top/gtfzigjnex.html

max(d, key=d.get)
来源：http://hz.kuanghao11.cn/gtbqasjcaq.html

[U10] Py：按值排序字典
来源：http://hz.bjfxy.top/gtnkyuylcu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtybhwvecn.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtmpovixcg.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtbwnyqywg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxinkj.top/gtdixjiuqz.html

Counter(arr).most_common(3)
来源：http://hz.zhiwuduotai.top/gtwxcwrpyd.html

[U13] Py：固定长度队列
来源：http://hz.svipenyu.cn/gtlpcoryiz.html

deque(maxlen=10)
来源：http://hz.aizwys.cn/gtjebhdnlb.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtczyfxajl.html

defaultdict(list)
来源：http://hz.hysaishi.cn/gtcnkdhuoa.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gttlpswxki.html

t = time.perf_counter()
来源：http://hz.shanyushiyangtech.top/gtyslbevpy.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtduubqbrp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtdsxoiyxh.html

[U17] Py：初始化日志
来源：http://hz.aibaodan.cn/gtvdootkbm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtjggpybrn.html

[U18] Py：预编译正则
来源：http://hz.bjfxy.top/gtdgsvucec.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gtuuzbdqxz.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtvyyfiffk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtujythwrl.html

[U20] Py：缓存函数结果
来源：http://hz.hnxiangtu.top/gtyoqnepej.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yueranfly.top/gtgxesreok.html

[U21] Py：自定义上下文管理器
来源：http://hz.zycfv.cn/gtaksrtout.html

@contextlib.contextmanager
来源：http://hz.zhixingplan.top/gtmqiajekb.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtdanjwwow.html

list(zip(*m))
来源：http://hz.cqqwz.cn/gtntiubuzz.html

[U23] Py：分块读取大文件
来源：http://hz.tian-w.cn/gtqhvxbrmu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.snrcjt.cn/gtkfhsutib.html

[U24] Py：路径操作
来源：http://hz.0kj1m.cn/gtkjksrkyd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hongshengwenyu.top/gttsubeqgi.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtpbzlqose.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtstptqrey.html

[U26] Py：并发下载
来源：http://hz.zycfv.cn/gtdmftucxo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtjlnrzaze.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtwlxmklra.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenlongwang.top/gtfsdlanyv.html

[U28] Py：类型别名
来源：http://hz.vqdsnc.cn/gtinitidwn.html

UserId = int
来源：http://hz.jiagoushi.top/gtrivhpazf.html

[U29] Py：属性校验
来源：http://hz.316326.xyz/gtmliyzlgb.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtatbtpdlk.html

[U30] Py：数据类
来源：http://hz.ivvv.top/gtniumrldc.html

@dataclass(slots=True)
来源：http://hz.sxryk.cn/gtuymctnjz.html

[U31] Py：单测
来源：http://hz.xinyue.icu/gtvjpgbqqb.html

python -m pytest -q
来源：http://hz.jinghuilouyu.cn/gtgtztvyqg.html

[U32] Py：代码格式化
来源：http://hz.hongshengwenyu.top/gtzvlaavth.html

ruff format . && ruff check --fix .
来源：http://hz.yueranfly.top/gthlheklaq.html

[U33] Py：打包发布
来源：http://hz.sufxvd.cn/gtsxgcyyzj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtdqkfukww.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gtygpkpsgj.html

chardet.detect(raw)
来源：http://hz.dianchejie.cn/gtdjrjnmhx.html

[U35] Py：发送邮件
来源：http://hz.daria6918.cn/gtgqmattmm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yangfankeji.com/gtrahklnob.html

[U36] Py：定时任务
来源：http://hz.andypj.xyz/gtkcgnqxll.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtsqfnkvwc.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gtntvdgzvf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtvsiwhpvr.html

[U38] Py：获取脚本所在目录
来源：http://hz.cqqwz.cn/gtwleotzys.html

Path(__file__).resolve().parent
来源：http://hz.redwolf501.top/gttsfszwll.html

[U39] Py：判断是否在交互环境
来源：http://hz.yvedp.cn/gtzvlfotou.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gthghtiuqk.html

[U40] Py：打印到标准错误
来源：http://hz.ehwqpu.com/gtzukndcjb.html

print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtdoececsl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guannengcc.top/gtpdihlftr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenjidiqi.icu/gtzkkddksp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yonumen.top/gtoryilumq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.316326.xyz/gtwjsmnupy.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtjmgwvxua.html

namespace App\Http;
来源：http://hz.yj20258.top/gtkhqfprkm.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258888.top/gtbepagleg.html

declare(strict_types=1);
来源：http://hz.zhoulong.xyz/gtzpagzvaa.html

[U45] PHP：类型声明与返回类型
来源：http://hz.mhx1999.top/gtuhtlnimj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtqnfdblyt.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtosbbzypv.html

?string $name = null
来源：http://hz.xylfe.cn/gttqxytfdx.html

[U47] PHP：联合类型
来源：http://hz.zhengqikj.top/gtmorrtldq.html

int|string $id
来源：http://hz.hnqzz.top/gtcgocltoh.html

[U48] PHP：纯枚举
来源：http://hz.aibaodan.cn/gtzzvfoqau.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtnovllvij.html

[U49] PHP：只读属性
来源：http://hz.jinghuilouyu.cn/gtbksvtjok.html

public readonly string $name
来源：http://hz.yj202588.top/gtgjnmevzi.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gttitgahlq.html

public function __construct(private int $id) {}
来源：http://hz.daxiang520.top/gtfjseydkd.html

[U51] PHP：数组解构
来源：http://hz.smart0.xyz/gtckvaaxzy.html

[$a, $b] = $arr;
来源：http://hz.cqqwz.cn/gtwpwxnkka.html

[U52] PHP：箭头函数
来源：http://hz.fengsongda.top/gtfpqaiwrs.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtnwtcalbe.html

[U53] PHP：空合并运算符
来源：http://hz.nanxinkj.top/gtmdpyywde.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gtkplfhxca.html

[U54] PHP：空安全调用
来源：http://hz.hongshengwenyu.top/gtbxtrpciy.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gthoeqrlsi.html

[U55] PHP：match 表达式
来源：http://hz.hywenlv.cn/gtpudfnmnz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhijiandao.cn/gtwziworlr.html

[U56] PHP：命名参数
来源：http://hz.zhoulong.xyz/gtwjjgubno.html

f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtvhvjjhpo.html

[U57] PHP：字符串插值
来源：http://hz.hammf.cn/gtpebvpdzv.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtcbbtnepk.html

[U58] PHP：数组三件套
来源：http://hz.hnxiangtu.top/gtkbsjpdac.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gtsgegpuvo.html

[U59] PHP：自定义排序
来源：http://hz.bjfxy.top/gtqmsiowzt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtdcfgbcvk.html

[U60] PHP：JSON 编解码
来源：http://hz.yanxiufei.cn/gtwgcmvojh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigfzy.top/gtovvstyot.html

[U61] PHP：正则
来源：http://hz.yj202588.top/gtxgbgphzz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtmevcoihk.html

[U62] PHP：日期对象
来源：http://hz.gaohongyu789.top/gtdvhelylc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtrxvdhued.html

[U63] PHP：文件读写
来源：http://hz.0kj1m.cn/gtuuoseizo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.guowangkeji.top/gtqyxbtexq.html

[U64] PHP：目录遍历
来源：http://hz.xuanzx.com/gtqmdhglrq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.dianchejie.cn/gtqoibnbsh.html

[U65] PHP：会话
来源：http://hz.jiagoushi.top/gtpwiishrm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gaohongyu789.top/gtwyxejvva.html

[U66] PHP：设置 Cookie
来源：http://hz.nwbrower.top/gtenxlzzzp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gtlunrbmdn.html

[U67] PHP：处理文件上传
来源：http://hz.xylfe.cn/gtwsuudopv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jqgufenzy.top/gtletqiugq.html

[U68] PHP：PDO 连接
来源：http://hz.nanxuanxn.top/gtvuqsekdw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj20258.top/gtufuvlelo.html

[U69] PHP：PDO 预处理
来源：http://hz.gogol.net.cn/gthnulwzbf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.daria6918.cn/gtqczhqydr.html

[U70] PHP：PDO 事务
来源：http://hz.nwbrower.top/gtmfajwisn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hongshengwenyu.top/gtdfsychbj.html

[U71] PHP：抛出异常
来源：http://hz.hywenlv.cn/gtvmjitqjl.html

throw new RuntimeException("失败", 500);
来源：http://hz.xziqi.cn/gtjwbprrty.html

[U72] PHP：写错误日志
来源：http://hz.yj20258888.top/gtnuuvagoi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.fengsongda.top/gtukeplpfx.html

[U73] PHP：读取 ini 配置
来源：http://hz.yueranfly.top/gtwwnghbue.html

parse_ini_file("config.ini", true)
来源：http://hz.9152youxi.cn/gttuiresce.html

[U74] PHP：读取环境变量
来源：http://hz.tianlin.xyz/gtrhwgemqf.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yuxming.cn/gtbhqyerca.html

[U75] PHP：依赖注入
来源：http://hz.yuanzhike.top/gteqvzpapv.html

composer require psr/container
来源：http://hz.xinyue.icu/gtgaonasqm.html

[U76] PHP：简单路由
来源：http://hz.dianchejie.cn/gtqfafgswd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.0kj1m.cn/gtsvezqjzm.html

[U77] PHP：模板渲染
来源：http://hz.zhengqikj.top/gtetdpdfqg.html

composer require twig/twig
来源：http://hz.hywenlv.cn/gtwblhdoyq.html

[U78] PHP：单元测试
来源：http://hz.feifeiyinyue.top/gtmqelplvi.html

composer require --dev phpunit/phpunit
来源：http://hz.jianghu66.top/gtqvrdbimb.html

[U79] PHP：静态分析
来源：http://hz.yj20258.top/gtenbrajcm.html

composer require --dev phpstan/phpstan
来源：http://hz.guowangkeji.top/gtebvtjbrd.html

[U80] PHP：代码规范修复
来源：http://hz.yonumen.top/gthllrgise.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zhiwuduotai.top/gtcyvauwcn.html

[U81] JS：初始化项目
来源：http://hz.dianchejie.cn/gtdfryjdam.html

npm init -y;  npm i express
来源：http://hz.hysaishi.cn/gtnvrphrsk.html

[U82] JS：package.json 脚本
来源：http://hz.smart0.xyz/gtxgvzzqeq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sweek.top/gtaopwtuqo.html

[U83] JS：ES Module 导入导出
来源：http://hz.daxiang520.top/gtbybhgojw.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yueranfly.top/gtfwfwckyw.html

[U84] JS：CommonJS 写法
来源：http://hz.guowangkeji.top/gtkdpoljdw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.sxryk.cn/gtuanoziba.html

[U85] JS：可选链
来源：http://hz.yongpay.top/gtyzczcphz.html

a?.b?.c
来源：http://hz.jinghuilouyu.cn/gtactnsnyf.html

[U86] JS：空值合并
来源：http://hz.pycfn.com/gtfvnrynrl.html

a ?? b
来源：http://hz.dianchejie.cn/gtyuzkohyu.html

[U87] JS：解构默认值
来源：http://hz.shangyingyoupin.top/gtnokifqkn.html

const { a = 1, b = 2 } = obj;
来源：http://hz.bjfxy.top/gtxtrcwhtb.html

[U88] JS：对象展开合并
来源：http://hz.hfpthk.cn/gtbshfduyw.html

{ ...a, ...b }
来源：http://hz.smart0.xyz/gtghuxdjdf.html

[U89] JS：数组去重
来源：http://hz.hammf.cn/gteplohacp.html

[...new Set(arr)]
来源：http://hz.sysykeji.top/gtcjyeupir.html

[U90] JS：数字数组排序
来源：http://hz.jqgfzy.top/gtnotyjjoy.html

[...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtcpoxwowe.html

[U91] JS：对象键值遍历
来源：http://hz.sufxvd.cn/gtalxyxzwq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.iojbl.cn/gtubguvmwa.html

[U92] JS：深拷贝
来源：http://hz.nanxinkj.top/gtfkxlblsb.html

structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtijsnagmp.html

[U93] JS：模板字符串
来源：http://hz.jyoumei.cn/gtulkuzhkj.html

`共 ${n} 条`
来源：http://hz.yuanzhike.top/gtwljvocjq.html

[U94] JS：箭头函数
来源：http://hz.zdqjudy.top/gtixlqeikl.html

const double = x => x * 2;
来源：http://hz.daxiang520.top/gtnmfzbfij.html

[U95] JS：Promise 包装
来源：http://hz.daria6918.cn/gtehzqqkra.html

new Promise((resolve, reject) => {})
来源：http://hz.zycfv.cn/gtnppxclbd.html

[U96] JS：async/await 与异常
来源：http://hz.guannengcc.top/gtvjrniujf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtvorbqaal.html

[U97] JS：并发请求
来源：http://hz.dashuyun.cn/gtwaewopat.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtsqwufrjd.html

[U98] JS：fetch 带 JSON
来源：http://hz.ivvv.top/gtyecuthsx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cqqwz.cn/gtwgzcmtpj.html

[U99] JS：事件监听
来源：http://hz.daria6918.cn/gtmpsybbut.html

el.addEventListener("click", e => {})
来源：http://hz.jianghu66.top/gtiukpiplu.html

[U100] JS：DOM 查询
来源：http://hz.xylfe.cn/gtktihobyn.html

document.querySelector(".item")
来源：http://hz.nwbrower.top/gtznweavjs.html

[U101] JS：classList 操作
来源：http://hz.bjfxy.top/gtijxqlqdm.html

el.classList.toggle("active")
来源：http://hz.jinghuilouyu.cn/gtyoaoupbm.html

[U102] JS：本地存储
来源：http://hz.52xcode.cn/gtrhprrhtx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yonumen.top/gtchnsidcv.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gtnjalhwiz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.tianlin.xyz/gtgvmdwoct.html

[U104] JS：防抖
来源：http://hz.chenlongwang.top/gtunluktuy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gtmusjkray.html

[U105] JS：节流
来源：http://hz.aizwys.cn/gtjvdcvidf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangdashe.top/gtugudihpi.html

[U106] JS：日期格式化
来源：http://hz.zhijiandao.cn/gtrmoeozbe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258888.top/gtiqqlfwjh.html

[U107] JS：数字千分位
来源：http://hz.zhijiandao.cn/gtgjthuktx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jqgufenzy.top/gtyxmwguqb.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gtajhijhlg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtcfmbkyxz.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtonwnvmca.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gtuyxvaksv.html

[U110] JS：数组分块
来源：http://hz.cheryme.top/gtfcmedahy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnqzz.top/gtxuizzbcg.html

[U111] JS：对象转 Map
来源：http://hz.yj20258.top/gtyaqttdrx.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtdwhvzkod.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtucloqxlx.html

"7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtkhhltybm.html

[U113] JS：正则替换全部
来源：http://hz.cdnleiting.top/gtusrcjocf.html

s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtfvamegai.html

[U114] JS：JSON 深比较
来源：http://hz.havefunace.top/gtsosxmicb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtimzhcjnu.html

[U115] JS：生成 UUID
来源：http://hz.jiagoushi.top/gtofvzmfiw.html

crypto.randomUUID()
来源：http://hz.zhijiandao.cn/gthmbyjkxj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shangyingyoupin.top/gtlejwgmzf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.mhx1999.top/gtuznaexyp.html

[U117] JS：单元测试
来源：http://hz.jqgfzy.top/gtjljhmpmc.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gtlppfmezb.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtjyhsodmh.html

npm i -D vite;  npx vite
来源：http://hz.chenjidiqi.icu/gteuftnhvv.html

[U119] JS：生产构建
来源：http://hz.yangfankeji.com/gtkghssiyl.html

npx vite build
来源：http://hz.gzhubu.top/gtkonmdfex.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shzxlz.cn/gtylfmpniu.html

import.meta.env.VITE_API_URL
来源：http://hz.jinghuilouyu.cn/gtdeoyeuji.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpmexhboi.html

统计汇总
来源：http://hz.sufxvd.cn/gtzvtmsbde.html

================================================================================
来源：http://hz.gzhubu.top/gtajtcgcve.html

按语言统计（条）：
来源：http://hz.ivvv.top/gthzmpxsdu.html

Python ......... 252
来源：http://hz.yj20258.top/gtwwliizgl.html

PHP ............ 252
来源：http://hz.xingfuxueyuan.xyz/gtccwbxiws.html

JavaScript ..... 252
来源：http://hz.fengsongda.top/gtguwfstqh.html

TypeScript ..... 212
来源：http://hz.hnxiangtu.top/gtclunpvsf.html

Java ........... 212
来源：http://hz.yj20258.top/gtjselqsbg.html

Go ............. 212
来源：http://hz.ydjk.org.cn/gtwrocsjiy.html

Ruby ........... 212
来源：http://hz.daxiang520.top/gtgvymuexv.html

C# ............. 212
来源：http://hz.cashguo.top/gtoqghquwg.html

C .............. 30
来源：http://hz.jyoumei.cn/gtakvsxfru.html

C++ ............ 30
来源：http://hz.guannengcc.top/gtnhehqkmi.html

SQL ............ 90
来源：http://hz.yanxiufei.cn/gtvphygsvm.html

Bash ........... 80
来源：http://hz.havefunace.top/gtmqykufnb.html

Kotlin ......... 15
来源：http://hz.birdmap.top/gthsnsfxne.html

Swift .......... 15
来源：http://hz.shanyushiyangkeji.top/gtagpnaihr.html

Lua ............ 10
来源：http://hz.hongshengwenyu.top/gtpxyuuwfk.html

Perl ........... 10
来源：http://hz.dianchejie.cn/gttnkwrnak.html

Scala .......... 10
来源：http://hz.jinghuilouyu.cn/gthcfqlagm.html

------------------------------------
来源：http://hz.yj20258.top/gtqoxqduck.html

合计 ........... 2106 条
来源：http://hz.yonumen.top/gtnuaawnqo.html

按章节统计：
来源：http://hz.ybcxt.top/gtnqcpnhcz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.birdmap.top/gtbgwifztg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtzytkrgqn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtpxjsfblh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtzkffajzp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.chenlongwang.top/gtbnbocxde.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.andypj.xyz/gtfmfbdooc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtibbyenhw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.meibo888.top/gtwdrtghtf.html


<!-- 参考信息 -->