代发 wailian999

[T49] Perl：函数
来源：http://hz.cucudq.cn/gtgljqepoz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.bjfxy.top/gtcjqmhhmf.html

[T50] Perl：逐行读文件
来源：http://hz.ehwqpu.com/gtynaclgud.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.iojbl.cn/gtklzvlldk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtcxugrgwm.html

[T51] Scala：Hello World
来源：http://hz.jinqigfzy.top/gtktufawzg.html

println("Hello")
来源：http://hz.hammf.cn/gttrhtowtv.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gthqzssghk.html

val a = 1;  var b = 2
来源：http://hz.zhiwuduotai.top/gtcldgeizy.html

[T53] Scala：字符串插值
来源：http://hz.cashguo.top/gtrhwwbqyd.html

s"值: $b"
来源：http://hz.yj202588.top/gtkacdzwba.html

[T54] Scala：集合映射
来源：http://hz.feifeiyinyue.top/gtpjdzyfyn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtljpyyehq.html

[T55] Scala：集合过滤
来源：http://hz.cheryme.top/gtgipyghmu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cqqwz.cn/gtoqrksmyi.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gtntfljrqk.html

case class User(name: String, age: Int)
来源：http://hz.jqgufenzy.top/gtepmtctno.html

[T57] Scala：模式匹配
来源：http://hz.jlsjyb.cn/gtrltuvwps.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yuanzhike.top/gtzbnldknn.html

[T58] Scala：函数定义
来源：http://hz.jinghuilouyu.cn/gttoodtswu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtnvnwqsut.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtdyiqrmyj.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gthtrwukwd.html

[T60] Scala：折叠
来源：http://hz.jinyuanbaomall.cn/gtjmcabuhh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sufxvd.cn/gtshonvios.html

================================================================================
来源：http://hz.yvedp.cn/gtxpwdftiq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtknncjauc.html

================================================================================
来源：http://hz.yj20258888.top/gtaualjjjz.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gtvgsaujgq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtfelfezpy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.vqdsnc.cn/gtjvftxwsq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinyuanbaomall.cn/gtexjbctzl.html

[U03] Py：加载 .env 配置
来源：http://hz.hysaishi.cn/gtimaxiwxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.iojbl.cn/gtkvtdrqxp.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtbiduzjvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtztclfwvj.html

[U05] Py：列表去重且保序
来源：http://hz.tianlin.xyz/gtixxyutbn.html

list(dict.fromkeys(arr))
来源：http://hz.ywan-chungtsiang.top/gtmeomgbyg.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gtianprhau.html

{**a, **b}
来源：http://hz.yueranfly.top/gtvgmijluf.html

[U07] Py：反转字典键值
来源：http://hz.daria6918.cn/gtbnhrziuy.html

{v: k for k, v in d.items()}
来源：http://hz.yuanzhike.top/gtlywqobqb.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtikecgdvm.html

[y for x in nested for y in x]
来源：http://hz.hnqzz.top/gtgboieiuq.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtjqpbmbwo.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtnulrzzgs.html

[U10] Py：按值排序字典
来源：http://hz.birdmap.top/gtlaygohmg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.quarkkingdee.top/gtsskskwbm.html

[U11] Py：生成器表达式
来源：http://hz.bjfxy.top/gtlqgrhjzt.html

(x * 2 for x in arr)
来源：http://hz.chenzaomai.com/gtqezhmknu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jqgufenzy.top/gtliszhndt.html

Counter(arr).most_common(3)
来源：http://hz.bjfxy.top/gtakhgidyy.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtgqmgdmqb.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtaakwchhi.html

[U14] Py：分组收集到列表
来源：http://hz.nwbrower.top/gtlaknwsfc.html

defaultdict(list)
来源：http://hz.yj202588.top/gtmvimiucd.html

[U15] Py：高精度计时
来源：http://hz.xinyue.icu/gtsqpnxdpv.html

t = time.perf_counter()
来源：http://hz.birdmap.top/gtyuaumqcy.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtakxmcerc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yonumen.top/gtthcextpi.html

[U17] Py：初始化日志
来源：http://hz.yvedp.cn/gtqyzplojt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj202588.top/gtnxqqsyrq.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangkeji.top/gtyxuweydw.html

pat = re.compile(r"\d+")
来源：http://hz.sufxvd.cn/gtuoifmcid.html

[U19] Py：正则替换带回调
来源：http://hz.jianghu66.top/gtnqqkpbjd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zycfv.cn/gtxiraszhp.html

[U20] Py：缓存函数结果
来源：http://hz.shzxlz.cn/gtazxcznzs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.meibo888.top/gtysnrgqru.html

[U21] Py：自定义上下文管理器
来源：http://hz.0kj1m.cn/gtaxibqois.html

@contextlib.contextmanager
来源：http://hz.xuetiantiany.cn/gthoulolxx.html

[U22] Py：矩阵转置
来源：http://hz.ybcxt.top/gtajcbcpqi.html

list(zip(*m))
来源：http://hz.ydzc1.top/gtijuujpxy.html

[U23] Py：分块读取大文件
来源：http://hz.jlsjyb.cn/gtrawjcfxo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daria6918.cn/gtshgfjqlo.html

[U24] Py：路径操作
来源：http://hz.haohaochexian.top/gtqpwumboi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gtokreyqrz.html

[U25] Py：CSV 按字典读
来源：http://hz.jianghu66.top/gtnioymwmq.html

csv.DictReader(f)
来源：http://hz.jyoumei.cn/gtwvxiprua.html

[U26] Py：并发下载
来源：http://hz.jinqigufen.top/gtzuxxupdo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtrejkpalr.html

[U27] Py：异步 HTTP
来源：http://hz.sufxvd.cn/gtxkpssrpm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ywan-chungtsiang.top/gtjujatfno.html

[U28] Py：类型别名
来源：http://hz.shangyingyoupin.top/gtvmzptzzd.html

UserId = int
来源：http://hz.iojbl.cn/gtiqwuojcx.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtmylspgrv.html

@property 与 @x.setter 配合
来源：http://hz.ybcxt.top/gtcukwofua.html

[U30] Py：数据类
来源：http://hz.chenlongwang.top/gtgzwnwney.html

@dataclass(slots=True)
来源：http://hz.jinghuilouyu.cn/gtwdrldwxg.html

[U31] Py：单测
来源：http://hz.tanke756.top/gttgxbyzhe.html

python -m pytest -q
来源：http://hz.dianchejie.cn/gtgjuzbvzy.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gtdipquhzb.html

ruff format . && ruff check --fix .
来源：http://hz.meibo888.top/gtcgkljmrt.html

[U33] Py：打包发布
来源：http://hz.dianchejie.cn/gtekwqowzg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ppjwa.cn/gtpyrhkpic.html

[U34] Py：判断编码
来源：http://hz.smart0.xyz/gtnkfjyqkh.html

chardet.detect(raw)
来源：http://hz.gotoacloud.top/gtnwqhgbfn.html

[U35] Py：发送邮件
来源：http://hz.gotoacloud.top/gtkmgzmwfs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.9152youxi.cn/gtfaxlvjut.html

[U36] Py：定时任务
来源：http://hz.hongshengwenyu.top/gtjgvlwsjx.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuanzhike.top/gtzaajbbvy.html

[U37] Py：读写 Excel
来源：http://hz.shanyushiyangtech.top/gtejnuqgyf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.316326.xyz/gtdnrevvcn.html

[U38] Py：获取脚本所在目录
来源：http://hz.dianchejie.cn/gtxvhkbpdu.html

Path(__file__).resolve().parent
来源：http://hz.ydzc1.top/gtrqgqyxxs.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuanzhike.top/gtvmpwnawu.html

sys.stdout.isatty()
来源：http://hz.wangshuangyany.cn/gtjbwouttt.html

[U40] Py：打印到标准错误
来源：http://hz.hywenlv.cn/gtagxdqmcm.html

print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtvwjizpux.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinghuilouyu.cn/gtrulojxfa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtexlcdqrd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgufenzy.top/gtfpwmgufk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuetiantiany.cn/gtxstmkskn.html

[U43] PHP：声明命名空间
来源：http://hz.xziqi.cn/gtznmyvoaj.html

namespace App\Http;
来源：http://hz.xuetiantiany.cn/gtzxdnesmk.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtpnffbfgh.html

declare(strict_types=1);
来源：http://hz.chenlongwang.top/gtujkuswyi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sweek.top/gtdxfixnxk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtwefkvjxf.html

[U46] PHP：可空类型
来源：http://hz.daxiang520.top/gtxrhctybt.html

?string $name = null
来源：http://hz.daxiang520.top/gticqfdmkk.html

[U47] PHP：联合类型
来源：http://hz.cashguo.top/gtyjdldnnr.html

int|string $id
来源：http://hz.jiagoushi.top/gtusjlddhl.html

[U48] PHP：纯枚举
来源：http://hz.ywan-chungtsiang.top/gttzwlpdye.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xziqi.cn/gtolrugqtr.html

[U49] PHP：只读属性
来源：http://hz.pengpengdd.cyou/gtgiiepavp.html

public readonly string $name
来源：http://hz.yangfankeji.com/gtfhohmmat.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gtsznfsqkd.html

public function __construct(private int $id) {}
来源：http://hz.cheryme.top/gtcqdtqmsy.html

[U51] PHP：数组解构
来源：http://hz.cheryme.top/gtvvbspgfh.html

[$a, $b] = $arr;
来源：http://hz.yj202588.top/gtiapbvovq.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtjxswqusw.html

$double = fn($x) => $x * 2;
来源：http://hz.zycfv.cn/gtbfgrpzdg.html

[U53] PHP：空合并运算符
来源：http://hz.yongpay.top/gtysgdhgsj.html

$v = $a ?? $b ?? "default";
来源：http://hz.cdnleiting.top/gtongvuhgf.html

[U54] PHP：空安全调用
来源：http://hz.gotoacloud.top/gtyknghkyi.html

$obj?->method()
来源：http://hz.iojbl.cn/gtdupkkwke.html

[U55] PHP：match 表达式
来源：http://hz.snrcjt.cn/gtzenetjhp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.iojbl.cn/gtuppwavnt.html

[U56] PHP：命名参数
来源：http://hz.sufxvd.cn/gtlvvgpigz.html

f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtbcfmtorc.html

[U57] PHP：字符串插值
来源：http://hz.cdnleiting.top/gtnagbetrj.html

"值: {$a}"
来源：http://hz.ehwqpu.com/gtjxjphgay.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtcldihdjv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.haohaochexian.top/gtxiyqwcww.html

[U59] PHP：自定义排序
来源：http://hz.jyoumei.cn/gttybcatbf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gttltzblvn.html

[U60] PHP：JSON 编解码
来源：http://hz.hnxiangtu.top/gtqnjsjizr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.vqdsnc.cn/gttkzjfmja.html

[U61] PHP：正则
来源：http://hz.chenjidiqi.icu/gtsjspblil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gthwbqgwgc.html

[U62] PHP：日期对象
来源：http://hz.yuxming.cn/gtnzjqclru.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhoulong.xyz/gtpaikwtll.html

[U63] PHP：文件读写
来源：http://hz.daxiang520.top/gtvbwqcqzd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhengqikj.top/gtdaohqozn.html

[U64] PHP：目录遍历
来源：http://hz.zhengqikj.top/gtwaromgef.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.smart0.xyz/gtlshpylmd.html

[U65] PHP：会话
来源：http://hz.jiagoushi.top/gtlomqynhp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.gotoacloud.top/gtcrqucrle.html

[U66] PHP：设置 Cookie
来源：http://hz.shzxlz.cn/gtufoiqlbo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.mhx1999.top/gttxkbdogm.html

[U67] PHP：处理文件上传
来源：http://hz.jqgufenzy.top/gthcryujkk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xylfe.cn/gtpjvysnxe.html

[U68] PHP：PDO 连接
来源：http://hz.shuidangran.top/gttlcyjrrf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.bjfxy.top/gtbqfhajhl.html

[U69] PHP：PDO 预处理
来源：http://hz.birdmap.top/gtnlfwzhug.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jianghu66.top/gtersnwipw.html

[U70] PHP：PDO 事务
来源：http://hz.yuxming.cn/gtzulydomx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnxiangtu.top/gtslynwxgb.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gtperpxbbb.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gtcamzubud.html

[U72] PHP：写错误日志
来源：http://hz.jianghu66.top/gtjnonjqcw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tian-w.cn/gtgubycspu.html

[U73] PHP：读取 ini 配置
来源：http://hz.gaohongyu789.top/gtolmaqfqs.html

parse_ini_file("config.ini", true)
来源：http://hz.chenzaomai.com/gteuzvjgdb.html

[U74] PHP：读取环境变量
来源：http://hz.feifeiyinyue.top/gtrpmzpaue.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shzxlz.cn/gtdxwhbncg.html

[U75] PHP：依赖注入
来源：http://hz.jinyuanbaomall.cn/gthvesngfe.html

composer require psr/container
来源：http://hz.yonumen.top/gtwstqwhea.html

[U76] PHP：简单路由
来源：http://hz.xuanzx.com/gtxhmwpcgd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangtech.top/gtpxgsnwfx.html

[U77] PHP：模板渲染
来源：http://hz.jianghu66.top/gtrvhkvvso.html

composer require twig/twig
来源：http://hz.jlsjyb.cn/gtsnfojcss.html

[U78] PHP：单元测试
来源：http://hz.daria6918.cn/gtixocjkrv.html

composer require --dev phpunit/phpunit
来源：http://hz.fzhhl.top/gtsqvsojbh.html

[U79] PHP：静态分析
来源：http://hz.wangdashe.top/gtscihkdiq.html

composer require --dev phpstan/phpstan
来源：http://hz.nanxinkj.top/gtpcevwfem.html

[U80] PHP：代码规范修复
来源：http://hz.nwbrower.top/gtvbsqcvjn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yuxming.cn/gtytfibogq.html

[U81] JS：初始化项目
来源：http://hz.bjfxy.top/gtygoyshjc.html

npm init -y;  npm i express
来源：http://hz.pengpengdd.cyou/gtyvojzqoy.html

[U82] JS：package.json 脚本
来源：http://hz.aizwys.cn/gtqqmwlshk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.chenlongwang.top/gtnlzdhhlk.html

[U83] JS：ES Module 导入导出
来源：http://hz.bjfxy.top/gtzmpawijz.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.smart0.xyz/gtrqwkowvo.html

[U84] JS：CommonJS 写法
来源：http://hz.yj202588.top/gtxkkfzwox.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.c1oappe.top/gtsaikytgl.html

[U85] JS：可选链
来源：http://hz.nanxinkj.top/gtevgknyid.html

a?.b?.c
来源：http://hz.zdqjudy.top/gtvvgvgjkr.html

[U86] JS：空值合并
来源：http://hz.hnxiangtu.top/gtjtnbhuet.html

a ?? b
来源：http://hz.snrcjt.cn/gtudemfhwh.html

[U87] JS：解构默认值
来源：http://hz.jqgufenzy.top/gtvjswngyz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.nwbrower.top/gtdypnkkwh.html

[U88] JS：对象展开合并
来源：http://hz.wangshuangyany.cn/gttcmtjkct.html

{ ...a, ...b }
来源：http://hz.shuidangran.top/gtgnmnvehc.html

[U89] JS：数组去重
来源：http://hz.zdqjudy.top/gtwqanzzvv.html

[...new Set(arr)]
来源：http://hz.svipenyu.cn/gtjwkgeytw.html

[U90] JS：数字数组排序
来源：http://hz.dashuyun.cn/gtahipxkmi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtwjxkmbkp.html

[U91] JS：对象键值遍历
来源：http://hz.zhixingplan.top/gtkxdempau.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.shzxlz.cn/gtzquqrode.html

[U92] JS：深拷贝
来源：http://hz.snrcjt.cn/gtbbhhpehh.html

structuredClone(obj)
来源：http://hz.c1oappe.top/gtfhqjzfgm.html

[U93] JS：模板字符串
来源：http://hz.ywan-chungtsiang.top/gtllmllaox.html

`共 ${n} 条`
来源：http://hz.fengsongda.top/gtmsyxazca.html

[U94] JS：箭头函数
来源：http://hz.hysaishi.cn/gtftibxfdl.html

const double = x => x * 2;
来源：http://hz.jiagoushi.top/gtgejifhri.html

[U95] JS：Promise 包装
来源：http://hz.quarkkingdee.top/gtqudvcgdj.html

new Promise((resolve, reject) => {})
来源：http://hz.andypj.xyz/gtggxoerpv.html

[U96] JS：async/await 与异常
来源：http://hz.yuxming.cn/gtovynmbdw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gttmrnzgal.html

[U97] JS：并发请求
来源：http://hz.pycfn.com/gtawdddkek.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtnwyluebh.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtnkhwfyzo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.daria6918.cn/gtxnopflmn.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gttrycrkbo.html

el.addEventListener("click", e => {})
来源：http://hz.daxiang520.top/gtsqvqsxob.html

[U100] JS：DOM 查询
来源：http://hz.zhaomingkeji.xyz/gtafrczvfo.html

document.querySelector(".item")
来源：http://hz.xuanzx.com/gtyeyrqyer.html

[U101] JS：classList 操作
来源：http://hz.birdmap.top/gttsatohwz.html

el.classList.toggle("active")
来源：http://hz.jlsjyb.cn/gtdegcqnfi.html

[U102] JS：本地存储
来源：http://hz.hnqzz.top/gtkyfspuyv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.yongpay.top/gtegcdqjrd.html

[U103] JS：定时器
来源：http://hz.jqgfzy.top/gtdgiannxh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sufxvd.cn/gtqjoxqcui.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtyzrtleop.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.wangshuangyany.cn/gtubtjukcg.html

[U105] JS：节流
来源：http://hz.sysykeji.top/gtaremkfeu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ydjk.org.cn/gtftwphyww.html

[U106] JS：日期格式化
来源：http://hz.smart0.xyz/gthselqyte.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zdqjudy.top/gtumkxjwaw.html

[U107] JS：数字千分位
来源：http://hz.zhixingplan.top/gtcavlzrmy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.wangdashe.top/gtwusfmqyo.html

[U108] JS：随机整数
来源：http://hz.xziqi.cn/gtttpdtuhx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.kuanghao11.cn/gtsnthsbsr.html

[U109] JS：数组分组
来源：http://hz.nanxuanxn.top/gtmrvaevsk.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gthipwvtez.html

[U110] JS：数组分块
来源：http://hz.jianghu66.top/gtxsvfblin.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sufxvd.cn/gtlabzxdgj.html

[U111] JS：对象转 Map
来源：http://hz.vqdsnc.cn/gtboldcfxn.html

new Map(Object.entries(obj))
来源：http://hz.kuanghao11.cn/gtsbycjgzg.html

[U112] JS：字符串补位
来源：http://hz.chenzaomai.com/gtoiwevnqn.html

"7".padStart(3, "0")
来源：http://hz.cashguo.top/gtyaqisuxy.html

[U113] JS：正则替换全部
来源：http://hz.jqgufenzy.top/gtyruwjnzw.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtvupjvrnx.html

[U114] JS：JSON 深比较
来源：http://hz.gotoacloud.top/gtyutivmnz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtqmzxoqis.html

[U115] JS：生成 UUID
来源：http://hz.gogol.net.cn/gtmgkozlou.html

crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gthbicgtmj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.haohaochexian.top/gtmtoexghl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.haohaochexian.top/gtaypyccbo.html

[U117] JS：单元测试
来源：http://hz.hfpthk.cn/gtqvgjttyp.html

npm i -D vitest;  npx vitest
来源：http://hz.zhongyouzk.top/gtdnojqpfw.html

[U118] JS：开发服务器
来源：http://hz.nanxuanxn.top/gtfrbggtke.html

npm i -D vite;  npx vite
来源：http://hz.nwbrower.top/gtlxzejxiv.html

[U119] JS：生产构建
来源：http://hz.chenlongwang.top/gtgjrtxotb.html

npx vite build
来源：http://hz.chenzaomai.com/gtsjatvdiq.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yvedp.cn/gtwddibwrr.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtjmvkuqgv.html

================================================================================
来源：http://hz.ydjk.org.cn/gtzrzdjvcj.html

统计汇总
来源：http://hz.bjfxy.top/gtagktcaby.html

================================================================================
来源：http://hz.tian-w.cn/gtchkxuhxj.html

按语言统计（条）：
来源：http://hz.yj202588.top/gtzlkeocwm.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtkmfqwhpx.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gteqaefbxc.html

JavaScript ..... 252
来源：http://hz.ydjk.org.cn/gtazyfvbat.html

TypeScript ..... 212
来源：http://hz.yuxming.cn/gtcxybvagp.html

Java ........... 212
来源：http://hz.snrcjt.cn/gtbcnemant.html

Go ............. 212
来源：http://hz.gaohongyu789.top/gtmogrichi.html

Ruby ........... 212
来源：http://hz.jqgufenzy.top/gtyhlfnyqi.html

C# ............. 212
来源：http://hz.aibaodan.cn/gtygdmjjsj.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtmqylhcmc.html

C++ ............ 30
来源：http://hz.bjfxy.top/gtpvqwvgla.html

SQL ............ 90
来源：http://hz.jlsjyb.cn/gtmfcmmofr.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gthojmsboh.html

Kotlin ......... 15
来源：http://hz.shanyushiyangkeji.top/gttmevcmmn.html

Swift .......... 15
来源：http://hz.zhiwuduotai.top/gtratlkxns.html

Lua ............ 10
来源：http://hz.haohaochexian.top/gtqwyfebck.html

Perl ........... 10
来源：http://hz.chenzaomai.com/gtjlaaerdy.html

Scala .......... 10
来源：http://hz.wangshuangyany.cn/gtwuhfiysl.html

------------------------------------
来源：http://hz.nanxinkj.top/gtsnotzdnw.html

合计 ........... 2106 条
来源：http://hz.pengpengdd.cyou/gtrmhhiydi.html

按章节统计：
来源：http://hz.chenzaomai.com/gtysjfqoox.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.svipenyu.cn/gtwvoufsaz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ppjwa.cn/gtiociocqc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtppawmxzr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.chenjidiqi.icu/gtliglcdjw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtficuctct.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtdshpkxya.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shanyushiyangtech.top/gtjkfphlch.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.xylfe.cn/gtjuvbaklz.html


<!-- 参考信息 -->