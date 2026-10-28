代发 wailian999

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtzxxlxwll.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtzhxjtzdw.html

[T50] Perl：逐行读文件
来源：http://hz.tianlin.xyz/gtxbhwgbig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tian-w.cn/gtvfpfcbyu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtsdajtrfl.html

[T51] Scala：Hello World
来源：http://hz.feifeiyinyue.top/gtypmwtest.html

println("Hello")
来源：http://hz.chenzaomai.com/gtgxluomzb.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtnggplfkm.html

val a = 1;  var b = 2
来源：http://hz.pycfn.com/gtsltwmdhj.html

[T53] Scala：字符串插值
来源：http://hz.zhongyouzk.top/gtdtcmzafd.html

s"值: $b"
来源：http://hz.dianchejie.cn/gtjjhupvxq.html

[T54] Scala：集合映射
来源：http://hz.zhengqikj.top/gtaelzxuqd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtmvtlllyg.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtikpgnmzy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.smart0.xyz/gtueywwahp.html

[T56] Scala：样例类
来源：http://hz.jiagoushi.top/gttlsxsgax.html

case class User(name: String, age: Int)
来源：http://hz.gzhubu.top/gtkjhpogyo.html

[T57] Scala：模式匹配
来源：http://hz.hywenlv.cn/gtnnpmhrsx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.0kj1m.cn/gtzcjcuguk.html

[T58] Scala：函数定义
来源：http://hz.nwbrower.top/gtlwkgfedj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.c1oappe.top/gtfcshlbab.html

[T59] Scala：循环
来源：http://hz.dianchejie.cn/gtbqjejpcl.html

for (i <- 1 to 10) println(i)
来源：http://hz.gaohongyu789.top/gtytlmldve.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtekmzdcub.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtcluxqfbf.html

================================================================================
来源：http://hz.tanke756.top/gtblnsivpd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gttofplwxi.html

================================================================================
来源：http://hz.shzxlz.cn/gtdstfwwae.html

[U01] Py：创建虚拟环境
来源：http://hz.52xcode.cn/gtkmsyplkz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtjuvrkdsp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtutpvpwcm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.svipenyu.cn/gtihffcrjt.html

[U03] Py：加载 .env 配置
来源：http://hz.pengpengdd.cyou/gttdpyhnnz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zycfv.cn/gtcojvhqzx.html

[U04] Py：变量调试打印
来源：http://hz.yueranfly.top/gtwqtuydjw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.feifeiyinyue.top/gtfahkgjhk.html

[U05] Py：列表去重且保序
来源：http://hz.andypj.xyz/gtyuxzxeoc.html

list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtoedhfsms.html

[U06] Py：合并两个字典
来源：http://hz.cashguo.top/gtboiehcmw.html

{**a, **b}
来源：http://hz.jiagoushi.top/gtnuycltrd.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtoyezhvad.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtmwwkthna.html

[U08] Py：展平二维列表
来源：http://hz.zhongyouzk.top/gtrrkkqnvn.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtaylznjjg.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtjwrvivip.html

max(d, key=d.get)
来源：http://hz.ivvv.top/gtgsvekkqz.html

[U10] Py：按值排序字典
来源：http://hz.yuanzhike.top/gtfmphtoek.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.mhx1999.top/gtrnvvclzy.html

[U11] Py：生成器表达式
来源：http://hz.gaohongyu789.top/gtrpwmjmhw.html

(x * 2 for x in arr)
来源：http://hz.gotoacloud.top/gtdyapaebr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zycfv.cn/gtavvcerff.html

Counter(arr).most_common(3)
来源：http://hz.wangshuangyany.cn/gtgqhyofxm.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtzlxujhds.html

deque(maxlen=10)
来源：http://hz.snrcjt.cn/gtljuhejis.html

[U14] Py：分组收集到列表
来源：http://hz.nanxinkj.top/gtfypdpwuf.html

defaultdict(list)
来源：http://hz.gotoacloud.top/gtmvwzgway.html

[U15] Py：高精度计时
来源：http://hz.vqdsnc.cn/gtxiyhcqka.html

t = time.perf_counter()
来源：http://hz.hfpthk.cn/gtcljhkhic.html

[U16] Py：命令行参数解析
来源：http://hz.cashguo.top/gtocfyfxbi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gtfspxwexl.html

[U17] Py：初始化日志
来源：http://hz.hnqzz.top/gtoheobnhi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.snrcjt.cn/gtmlzsgskg.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangkeji.top/gttbliyqhh.html

pat = re.compile(r"\d+")
来源：http://hz.yanxiufei.cn/gtcrmotpgn.html

[U19] Py：正则替换带回调
来源：http://hz.svipenyu.cn/gtewgyyyhg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtpbbavbsa.html

[U20] Py：缓存函数结果
来源：http://hz.ydzc1.top/gtsnhmtbqw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258.top/gtqhkfgtlg.html

[U21] Py：自定义上下文管理器
来源：http://hz.hfpthk.cn/gtczgcoqjc.html

@contextlib.contextmanager
来源：http://hz.snrcjt.cn/gtmipzyguf.html

[U22] Py：矩阵转置
来源：http://hz.daria6918.cn/gtvsfdqgel.html

list(zip(*m))
来源：http://hz.ivvv.top/gtagdsxsho.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigfzy.top/gtkykoahlf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtwjvvwsys.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtvewjkeng.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.vqdsnc.cn/gtnvliqrso.html

[U25] Py：CSV 按字典读
来源：http://hz.xuanzx.com/gtfuhzjkhk.html

csv.DictReader(f)
来源：http://hz.nanxuanxn.top/gtdznhpjml.html

[U26] Py：并发下载
来源：http://hz.yj202588.top/gtnkmhakkp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hongshengwenyu.top/gtpdjguytw.html

[U27] Py：异步 HTTP
来源：http://hz.dianchejie.cn/gtgpexsfoh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gtstaicjlv.html

[U28] Py：类型别名
来源：http://hz.xuanzx.com/gtjbtfwhgi.html

UserId = int
来源：http://hz.redwolf501.top/gtazacjmws.html

[U29] Py：属性校验
来源：http://hz.fengsongda.top/gtccdrlxhi.html

@property 与 @x.setter 配合
来源：http://hz.guowangkeji.top/gtjxhxyqgt.html

[U30] Py：数据类
来源：http://hz.zhixingplan.top/gtnlsimuei.html

@dataclass(slots=True)
来源：http://hz.ydjk.org.cn/gticlbfrbq.html

[U31] Py：单测
来源：http://hz.xziqi.cn/gttbaublca.html

python -m pytest -q
来源：http://hz.hfpthk.cn/gtlkfqrniq.html

[U32] Py：代码格式化
来源：http://hz.birdmap.top/gtgymfmrwn.html

ruff format . && ruff check --fix .
来源：http://hz.nanxuanxn.top/gtjaudgsaj.html

[U33] Py：打包发布
来源：http://hz.ivvv.top/gtnxtwhnax.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.smart0.xyz/gtftuokyuk.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtalvuohhk.html

chardet.detect(raw)
来源：http://hz.gogol.net.cn/gtdiiybcvl.html

[U35] Py：发送邮件
来源：http://hz.cashguo.top/gtfjfbkerz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gttkzzdrir.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtmbyicyxc.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtqweikdkl.html

[U37] Py：读写 Excel
来源：http://hz.yj202588.top/gtnbfnxggt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.316326.xyz/gtxueizlld.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gthuvitlhx.html

Path(__file__).resolve().parent
来源：http://hz.wangshuangyany.cn/gtgdnxxlfz.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenzaomai.com/gtsqqkgfax.html

sys.stdout.isatty()
来源：http://hz.xingfuxueyuan.xyz/gtmmsyzszk.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtgniyowah.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtzcfftlry.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtmhraralc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhixingplan.top/gtdntxsuxo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtvtzhhzts.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.redwolf501.top/gtffjybbke.html

[U43] PHP：声明命名空间
来源：http://hz.bjfxy.top/gtrjtejhof.html

namespace App\Http;
来源：http://hz.nanxinkj.top/gtjyaiivsy.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gttzkcunpq.html

declare(strict_types=1);
来源：http://hz.bjfxy.top/gtqrezkadd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pycfn.com/gtsonknhda.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtpndgdfmo.html

[U46] PHP：可空类型
来源：http://hz.birdmap.top/gtorzwznhz.html

?string $name = null
来源：http://hz.yueranfly.top/gtthixechn.html

[U47] PHP：联合类型
来源：http://hz.yanxiufei.cn/gtighbhqpv.html

int|string $id
来源：http://hz.yj202588.top/gtfadapywu.html

[U48] PHP：纯枚举
来源：http://hz.daria6918.cn/gtkmrhimjt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtfkbkmane.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtjshqoqnw.html

public readonly string $name
来源：http://hz.yanxiufei.cn/gtbuzmrknb.html

[U50] PHP：构造器属性提升
来源：http://hz.fzhhl.top/gtmvhaydvg.html

public function __construct(private int $id) {}
来源：http://hz.wangshuangyany.cn/gtdwgoqvss.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtvjoulkwp.html

[$a, $b] = $arr;
来源：http://hz.nwbrower.top/gtqgrlfhlt.html

[U52] PHP：箭头函数
来源：http://hz.dashuyun.cn/gtfkvlnozv.html

$double = fn($x) => $x * 2;
来源：http://hz.hnxiangtu.top/gtxrohernm.html

[U53] PHP：空合并运算符
来源：http://hz.bjfxy.top/gttsslfuzp.html

$v = $a ?? $b ?? "default";
来源：http://hz.0kj1m.cn/gtxpbrtqie.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtbbiirsty.html

$obj?->method()
来源：http://hz.cashguo.top/gtfknhjiah.html

[U55] PHP：match 表达式
来源：http://hz.ehwqpu.com/gtnqlznhpn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sufxvd.cn/gtblzgjfmx.html

[U56] PHP：命名参数
来源：http://hz.andypj.xyz/gtajkxfyhw.html

f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtuuwjtteg.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtaoenzmhg.html

"值: {$a}"
来源：http://hz.dianchejie.cn/gtpzavnvnx.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtigrujqok.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aizwys.cn/gtnyaerrcu.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtzdnnywhc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtzkojildr.html

[U60] PHP：JSON 编解码
来源：http://hz.birdmap.top/gtunwykqjl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgufenzy.top/gttermktjv.html

[U61] PHP：正则
来源：http://hz.chenlongwang.top/gtvulpiqte.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtihchvrnx.html

[U62] PHP：日期对象
来源：http://hz.pycfn.com/gtzvdhgijr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangdashe.top/gtcxmiudbe.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtynvtcdqs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinqigufen.top/gtwvdbqxii.html

[U64] PHP：目录遍历
来源：http://hz.jianghu66.top/gtjgwlpegs.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtxivrvwey.html

[U65] PHP：会话
来源：http://hz.yj20258.top/gtgaawcjtz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.vqdsnc.cn/gtdwrzgpnf.html

[U66] PHP：设置 Cookie
来源：http://hz.guannengcc.top/gtzzqxvbre.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydjk.org.cn/gtovsrzsei.html

[U67] PHP：处理文件上传
来源：http://hz.kuanghao11.cn/gteshxaove.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxinkj.top/gtnhwttpar.html

[U68] PHP：PDO 连接
来源：http://hz.xingfuxueyuan.xyz/gtxmlcnciy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shangyingyoupin.top/gtcvqhuqnj.html

[U69] PHP：PDO 预处理
来源：http://hz.tian-w.cn/gtrroffeph.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yvedp.cn/gtkzsffdxw.html

[U70] PHP：PDO 事务
来源：http://hz.tianlin.xyz/gtkyvmxjas.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.dashuyun.cn/gtvaqnaakd.html

[U71] PHP：抛出异常
来源：http://hz.guowangkeji.top/gtrdhfmtwv.html

throw new RuntimeException("失败", 500);
来源：http://hz.xuanzx.com/gtzoinltug.html

[U72] PHP：写错误日志
来源：http://hz.xziqi.cn/gtjmmegxnn.html

error_log("失败: " . $e->getMessage());
来源：http://hz.iojbl.cn/gtwxhwvzqo.html

[U73] PHP：读取 ini 配置
来源：http://hz.ivvv.top/gtayiuamvi.html

parse_ini_file("config.ini", true)
来源：http://hz.cashguo.top/gtttgdufuv.html

[U74] PHP：读取环境变量
来源：http://hz.havefunace.top/gtitjoexul.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xuanzx.com/gthznyjxll.html

[U75] PHP：依赖注入
来源：http://hz.nanxinkj.top/gtjapxmtju.html

composer require psr/container
来源：http://hz.smart0.xyz/gttkvxmoci.html

[U76] PHP：简单路由
来源：http://hz.hfpthk.cn/gtkqmdfvhf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.dashuyun.cn/gtqrvrflgh.html

[U77] PHP：模板渲染
来源：http://hz.ybcxt.top/gtnqvfsczm.html

composer require twig/twig
来源：http://hz.gotoacloud.top/gtxlxencgc.html

[U78] PHP：单元测试
来源：http://hz.yangfankeji.com/gtotdibvvo.html

composer require --dev phpunit/phpunit
来源：http://hz.zhengqikj.top/gtcemprxqz.html

[U79] PHP：静态分析
来源：http://hz.zhaomingkeji.xyz/gtfyqsdisz.html

composer require --dev phpstan/phpstan
来源：http://hz.gaohongyu789.top/gtujafptzr.html

[U80] PHP：代码规范修复
来源：http://hz.pycfn.com/gtxgdudhqw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.fengsongda.top/gtaxphpoqu.html

[U81] JS：初始化项目
来源：http://hz.guowangkeji.top/gtlrtunllt.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtktyukopc.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtfgsztvsm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinyuanbaomall.cn/gtinokomkn.html

[U83] JS：ES Module 导入导出
来源：http://hz.shuidangran.top/gtnaqhaisy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.tanke756.top/gtdsyiiuza.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtzgcqcnnz.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.haohaochexian.top/gtghtvymim.html

[U85] JS：可选链
来源：http://hz.yj202588.top/gtroieyrfv.html

a?.b?.c
来源：http://hz.gogol.net.cn/gtevtvyaao.html

[U86] JS：空值合并
来源：http://hz.bjfxy.top/gtjtjlypet.html

a ?? b
来源：http://hz.yangfankeji.com/gtmpqgvsdx.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtylbjlmhr.html

const { a = 1, b = 2 } = obj;
来源：http://hz.vqdsnc.cn/gthywmjwdm.html

[U88] JS：对象展开合并
来源：http://hz.tianlin.xyz/gtkovnonyi.html

{ ...a, ...b }
来源：http://hz.jinqigufen.top/gtypoiyjcw.html

[U89] JS：数组去重
来源：http://hz.ywan-chungtsiang.top/gtkyoanalb.html

[...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtbtzorlxd.html

[U90] JS：数字数组排序
来源：http://hz.gogol.net.cn/gtiphamyae.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtwctcvxfc.html

[U91] JS：对象键值遍历
来源：http://hz.mhx1999.top/gtppkuhlqr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hnxiangtu.top/gtgvjnqqvs.html

[U92] JS：深拷贝
来源：http://hz.hammf.cn/gtgfjptgrj.html

structuredClone(obj)
来源：http://hz.redwolf501.top/gtokndgvhb.html

[U93] JS：模板字符串
来源：http://hz.hysaishi.cn/gtonozmvrp.html

`共 ${n} 条`
来源：http://hz.aibaodan.cn/gtddavnemu.html

[U94] JS：箭头函数
来源：http://hz.316326.xyz/gtkcsxmoup.html

const double = x => x * 2;
来源：http://hz.yueranfly.top/gtotrantix.html

[U95] JS：Promise 包装
来源：http://hz.chenjidiqi.icu/gttsjwnsbw.html

new Promise((resolve, reject) => {})
来源：http://hz.9152youxi.cn/gtfsphfgvq.html

[U96] JS：async/await 与异常
来源：http://hz.jqgufenzy.top/gtzafsusez.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.guowangkeji.top/gtgtwtslxu.html

[U97] JS：并发请求
来源：http://hz.xingfuxueyuan.xyz/gttrrgbugu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtrgfmnuau.html

[U98] JS：fetch 带 JSON
来源：http://hz.jqgfzy.top/gtgmcqsqgb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yvedp.cn/gthhdwblgt.html

[U99] JS：事件监听
来源：http://hz.ivvv.top/gtatupyzmw.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258.top/gtefaarvxx.html

[U100] JS：DOM 查询
来源：http://hz.feifeiyinyue.top/gtrbalewqu.html

document.querySelector(".item")
来源：http://hz.bjfxy.top/gtumvcetnl.html

[U101] JS：classList 操作
来源：http://hz.cdnleiting.top/gtjyrfyrxg.html

el.classList.toggle("active")
来源：http://hz.shangyingyoupin.top/gtyjzxzvbc.html

[U102] JS：本地存储
来源：http://hz.gogol.net.cn/gtazfyqiby.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ppjwa.cn/gtiqgfjtrs.html

[U103] JS：定时器
来源：http://hz.hnqzz.top/gtpoxmiyef.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenjidiqi.icu/gtpbkqdras.html

[U104] JS：防抖
来源：http://hz.jyoumei.cn/gtnmrtelkd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtjctqhuha.html

[U105] JS：节流
来源：http://hz.jyoumei.cn/gttilldfjl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jinqigufen.top/gtpvnnvxch.html

[U106] JS：日期格式化
来源：http://hz.gaohongyu789.top/gtzheeqrmw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.pengpengdd.cyou/gtlgprwfys.html

[U107] JS：数字千分位
来源：http://hz.smart0.xyz/gtftlwguxb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.dianchejie.cn/gttsfllehr.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtczsnvezs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yonumen.top/gtlgesjwhj.html

[U109] JS：数组分组
来源：http://hz.gotoacloud.top/gtukbnuyvb.html

Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtnfyyqxbn.html

[U110] JS：数组分块
来源：http://hz.cqqwz.cn/gthbsqwcfr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydzc1.top/gtaaznsbmb.html

[U111] JS：对象转 Map
来源：http://hz.xinyue.icu/gtkggguzet.html

new Map(Object.entries(obj))
来源：http://hz.yongpay.top/gtqcwixmrr.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtdyqjpihz.html

"7".padStart(3, "0")
来源：http://hz.sweek.top/gtuzhjusbo.html

[U113] JS：正则替换全部
来源：http://hz.bjfxy.top/gthxhplrkt.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtgkspdxpt.html

[U114] JS：JSON 深比较
来源：http://hz.ehwqpu.com/gtyyssieng.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtyxdeeekf.html

[U115] JS：生成 UUID
来源：http://hz.quarkkingdee.top/gtaqxdqqxb.html

crypto.randomUUID()
来源：http://hz.xuanzx.com/gtlaayfzfu.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gzhubu.top/gtgrtbksiu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tanke756.top/gtffwqgwqf.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangtech.top/gtcybzpruz.html

npm i -D vitest;  npx vitest
来源：http://hz.haohaochexian.top/gtccpwkdqa.html

[U118] JS：开发服务器
来源：http://hz.xziqi.cn/gtdrexgtts.html

npm i -D vite;  npx vite
来源：http://hz.xuetiantiany.cn/gtugvgldpa.html

[U119] JS：生产构建
来源：http://hz.zhijiandao.cn/gtlsrhdntf.html

npx vite build
来源：http://hz.316326.xyz/gtcfcyglmj.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yongpay.top/gtdfneujax.html

import.meta.env.VITE_API_URL
来源：http://hz.sweek.top/gtniaqyjvd.html

================================================================================
来源：http://hz.cashguo.top/gtfnuhextc.html

统计汇总
来源：http://hz.fengsongda.top/gtxgkcatox.html

================================================================================
来源：http://hz.shzxlz.cn/gtxjritwyp.html

按语言统计（条）：
来源：http://hz.zhiwuduotai.top/gtmzqbjtsx.html

Python ......... 252
来源：http://hz.mhx1999.top/gtjomlklem.html

PHP ............ 252
来源：http://hz.quarkkingdee.top/gtkdqtakhf.html

JavaScript ..... 252
来源：http://hz.yonumen.top/gtjppfwdqz.html

TypeScript ..... 212
来源：http://hz.bjfxy.top/gtxskorwby.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtyfwlxymy.html

Go ............. 212
来源：http://hz.hnqzz.top/gtaelgwwvy.html

Ruby ........... 212
来源：http://hz.yangfankeji.com/gtdvdxadbg.html

C# ............. 212
来源：http://hz.feifeiyinyue.top/gtfzkfavos.html

C .............. 30
来源：http://hz.316326.xyz/gtjlkweczw.html

C++ ............ 30
来源：http://hz.9152youxi.cn/gtsdtnfydo.html

SQL ............ 90
来源：http://hz.ehwqpu.com/gtizbuvnep.html

Bash ........... 80
来源：http://hz.redwolf501.top/gtqjvndubb.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gtjsjdiyqu.html

Swift .......... 15
来源：http://hz.tianlin.xyz/gtkbfpmiuh.html

Lua ............ 10
来源：http://hz.birdmap.top/gtdyzpivea.html

Perl ........... 10
来源：http://hz.dianchejie.cn/gtvwncivsx.html

Scala .......... 10
来源：http://hz.wangshuangyany.cn/gtrrxealoi.html

------------------------------------
来源：http://hz.hnqzz.top/gtzdfxdxst.html

合计 ........... 2106 条
来源：http://hz.yuxming.cn/gtsbyvckdt.html

按章节统计：
来源：http://hz.chenlongwang.top/gtmvibeack.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258.top/gtbkdzdaex.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ybcxt.top/gtzsresgoq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtfykyuiod.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gzhubu.top/gtjbexkcyh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.birdmap.top/gtrcwqigyy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nwbrower.top/gthexxqxri.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtopyquwkx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gtolblpfql.html


<!-- 参考信息 -->