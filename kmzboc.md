代发 wailian999

[T49] Perl：函数
来源：http://hz.gzhubu.top/gtsvilfgea.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtjwalczwo.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtruycykfk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.vqdsnc.cn/gttwjfyisc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhoulong.xyz/gtbdhqywov.html

[T51] Scala：Hello World
来源：http://hz.nwbrower.top/gtycjgmvvg.html

println("Hello")
来源：http://hz.ppjwa.cn/gtucsfgcqg.html

[T52] Scala：变量
来源：http://hz.sysykeji.top/gtdshxzwza.html

val a = 1;  var b = 2
来源：http://hz.zhongyouzk.top/gtpmwveixe.html

[T53] Scala：字符串插值
来源：http://hz.hammf.cn/gtlzgtshyo.html

s"值: $b"
来源：http://hz.sufxvd.cn/gtrarjxmss.html

[T54] Scala：集合映射
来源：http://hz.tian-w.cn/gtnpitfuyp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhongyouzk.top/gtjbogyade.html

[T55] Scala：集合过滤
来源：http://hz.wangshuangyany.cn/gtgclqpgtn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhiwuduotai.top/gtwewuhuxu.html

[T56] Scala：样例类
来源：http://hz.wangdashe.top/gtnsuwecex.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gtouorpmmr.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtnsrsoefn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.aibaodan.cn/gtdbbsinsi.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtijwwssfc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinyuanbaomall.cn/gtyzbatjoo.html

[T59] Scala：循环
来源：http://hz.jqgufenzy.top/gtopuafbsr.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtaefwqhta.html

[T60] Scala：折叠
来源：http://hz.yonumen.top/gtjbfqychh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dianchejie.cn/gtxxlliqtq.html

================================================================================
来源：http://hz.sweek.top/gtcjszqvub.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtosepcceg.html

================================================================================
来源：http://hz.yonumen.top/gtgouqxqbx.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtxhgqvfuv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenzaomai.com/gtpudusemw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jlsjyb.cn/gtioezgptq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xinyue.icu/gtlyehduys.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtykjiwqwp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtgfqtohcp.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtekzwsgor.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zycfv.cn/gtlokzobko.html

[U05] Py：列表去重且保序
来源：http://hz.ehwqpu.com/gthykzstlc.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtqcvfnxkb.html

[U06] Py：合并两个字典
来源：http://hz.0kj1m.cn/gtznsqhfdw.html

{**a, **b}
来源：http://hz.hysaishi.cn/gtihgailqq.html

[U07] Py：反转字典键值
来源：http://hz.cqqwz.cn/gteorymfvx.html

{v: k for k, v in d.items()}
来源：http://hz.shuidangran.top/gtvmaxopik.html

[U08] Py：展平二维列表
来源：http://hz.ywan-chungtsiang.top/gtexscofym.html

[y for x in nested for y in x]
来源：http://hz.chenjidiqi.icu/gtozcgjdsn.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigufen.top/gtqoyjxeam.html

max(d, key=d.get)
来源：http://hz.sweek.top/gtdjawjiif.html

[U10] Py：按值排序字典
来源：http://hz.0kj1m.cn/gtfagtxppz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.svipenyu.cn/gtqqoddrrm.html

[U11] Py：生成器表达式
来源：http://hz.ppjwa.cn/gttqcejcch.html

(x * 2 for x in arr)
来源：http://hz.gzhubu.top/gtdcnpbcuw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhixingplan.top/gtmmwjdeyr.html

Counter(arr).most_common(3)
来源：http://hz.dianchejie.cn/gtlsncaecc.html

[U13] Py：固定长度队列
来源：http://hz.xuetiantiany.cn/gtrfcifzhi.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtaknqofcd.html

[U14] Py：分组收集到列表
来源：http://hz.guowangkeji.top/gtzcggjiqa.html

defaultdict(list)
来源：http://hz.gaohongyu789.top/gtdukzktup.html

[U15] Py：高精度计时
来源：http://hz.ydzc1.top/gtsyxybqbs.html

t = time.perf_counter()
来源：http://hz.hongshengwenyu.top/gtvcrsohgc.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gtorymzwfe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258.top/gtylzddxgu.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gtbhzcehuv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgfzy.top/gtohujlfkw.html

[U18] Py：预编译正则
来源：http://hz.zhiwuduotai.top/gttzelqlyn.html

pat = re.compile(r"\d+")
来源：http://hz.birdmap.top/gtmsetitut.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gtlorwskwt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pengpengdd.cyou/gtwlesaktp.html

[U20] Py：缓存函数结果
来源：http://hz.hnxiangtu.top/gtdskixxfi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sweek.top/gtdmblehws.html

[U21] Py：自定义上下文管理器
来源：http://hz.cashguo.top/gtjaewfsaa.html

@contextlib.contextmanager
来源：http://hz.yuxming.cn/gtrivmsxgv.html

[U22] Py：矩阵转置
来源：http://hz.chenjidiqi.icu/gtqxmamwsj.html

list(zip(*m))
来源：http://hz.sxryk.cn/gtyhvtwhww.html

[U23] Py：分块读取大文件
来源：http://hz.iojbl.cn/gtyqqhtqsz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zdqjudy.top/gtlmwdzmxf.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gterwfmvst.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtsxeskcuw.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gttlgoetkk.html

csv.DictReader(f)
来源：http://hz.c1oappe.top/gtcfzvbngz.html

[U26] Py：并发下载
来源：http://hz.guannengcc.top/gtkntpfmca.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gthfwxtyer.html

[U27] Py：异步 HTTP
来源：http://hz.andypj.xyz/gtdgmtpgio.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gtnpuokpco.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtqirvsjnr.html

UserId = int
来源：http://hz.yangfankeji.com/gtcmkvuyuj.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gtdsizfaxp.html

@property 与 @x.setter 配合
来源：http://hz.c1oappe.top/gttxxtpqhn.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtzcddmwbr.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangkeji.top/gttdncbivs.html

[U31] Py：单测
来源：http://hz.iojbl.cn/gtkesbxhmw.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gtszbbfewo.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangtech.top/gtvygfetke.html

ruff format . && ruff check --fix .
来源：http://hz.aizwys.cn/gtecipnudd.html

[U33] Py：打包发布
来源：http://hz.jinyuanbaomall.cn/gtadmhrrow.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinyuanbaomall.cn/gtpeesmrya.html

[U34] Py：判断编码
来源：http://hz.redwolf501.top/gtlnazvfbq.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtwoscbxuu.html

[U35] Py：发送邮件
来源：http://hz.daria6918.cn/gtyzoraofr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tianlin.xyz/gtdmfmvgby.html

[U36] Py：定时任务
来源：http://hz.yj20258888.top/gtdrbnkjcs.html

schedule.every(10).minutes.do(job)
来源：http://hz.cqqwz.cn/gtgwutvost.html

[U37] Py：读写 Excel
来源：http://hz.chenzaomai.com/gtulprkgii.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gteiewfehk.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtvqkyqyza.html

Path(__file__).resolve().parent
来源：http://hz.ybcxt.top/gtpfjlyuqq.html

[U39] Py：判断是否在交互环境
来源：http://hz.andypj.xyz/gtrxbloaki.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtiddfcdtr.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gtvaeyajho.html

print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gthuwqvnvx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnxiangtu.top/gtqomurequ.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtlotiyapm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.svipenyu.cn/gttxdyuodb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fzhhl.top/gtudmceeqc.html

[U43] PHP：声明命名空间
来源：http://hz.cashguo.top/gtnulwlbku.html

namespace App\Http;
来源：http://hz.dianchejie.cn/gtzgwumvyc.html

[U44] PHP：开启严格类型
来源：http://hz.snrcjt.cn/gtwkzhxbts.html

declare(strict_types=1);
来源：http://hz.0kj1m.cn/gtzicxlsbr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yanxiufei.cn/gtfamblrea.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gttxxhkfmt.html

[U46] PHP：可空类型
来源：http://hz.jinqigfzy.top/gtqhkjiafs.html

?string $name = null
来源：http://hz.hywenlv.cn/gtgeiehctb.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtkytilrup.html

int|string $id
来源：http://hz.yueranfly.top/gtayapkxwj.html

[U48] PHP：纯枚举
来源：http://hz.ppjwa.cn/gtlyamgldt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtqgqkqztn.html

[U49] PHP：只读属性
来源：http://hz.hnqzz.top/gtyystjald.html

public readonly string $name
来源：http://hz.jinghuilouyu.cn/gtsmqclpbs.html

[U50] PHP：构造器属性提升
来源：http://hz.tian-w.cn/gterjxtqpp.html

public function __construct(private int $id) {}
来源：http://hz.ybcxt.top/gtodemzfag.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangtech.top/gtwaggayfk.html

[$a, $b] = $arr;
来源：http://hz.c1oappe.top/gtgyvavkoa.html

[U52] PHP：箭头函数
来源：http://hz.zhaomingkeji.xyz/gtxujwsfzi.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtybbfomrq.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtbeavucmu.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangshuangyany.cn/gtyajhonee.html

[U54] PHP：空安全调用
来源：http://hz.ydzc1.top/gtfooxiahs.html

$obj?->method()
来源：http://hz.fengsongda.top/gttqucypgx.html

[U55] PHP：match 表达式
来源：http://hz.jinqigufen.top/gtsapdvtog.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jiagoushi.top/gtqrbykwmv.html

[U56] PHP：命名参数
来源：http://hz.shangyingyoupin.top/gtkocxkewa.html

f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtajzwzxkh.html

[U57] PHP：字符串插值
来源：http://hz.c1oappe.top/gtpxvmytvx.html

"值: {$a}"
来源：http://hz.pengpengdd.cyou/gtiprcxauz.html

[U58] PHP：数组三件套
来源：http://hz.ydjk.org.cn/gtpsjyacic.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tanke756.top/gtghovqred.html

[U59] PHP：自定义排序
来源：http://hz.yanxiufei.cn/gtjqzwshdr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtfgbtrfwi.html

[U60] PHP：JSON 编解码
来源：http://hz.xuanzx.com/gtzoelysgs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.feifeiyinyue.top/gtjnyfzrzw.html

[U61] PHP：正则
来源：http://hz.smart0.xyz/gtcpyspqdl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtmmxsgqwn.html

[U62] PHP：日期对象
来源：http://hz.yuanzhike.top/gtqtzigngx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gtvngjdpsx.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtbaaadmvm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.haohaochexian.top/gtjmoyvubk.html

[U64] PHP：目录遍历
来源：http://hz.yanxiufei.cn/gtribdwtqs.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.haohaochexian.top/gtihclrqkz.html

[U65] PHP：会话
来源：http://hz.cucudq.cn/gtfevkpiqc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.tanke756.top/gtfjbdyavg.html

[U66] PHP：设置 Cookie
来源：http://hz.yj202588.top/gttgunpajv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nwbrower.top/gtakbcuapx.html

[U67] PHP：处理文件上传
来源：http://hz.dianchejie.cn/gtjnrqvirz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zycfv.cn/gtcohvmcgx.html

[U68] PHP：PDO 连接
来源：http://hz.zhengqikj.top/gtfgejlnnv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xuanzx.com/gtpcpsbyoc.html

[U69] PHP：PDO 预处理
来源：http://hz.haohaochexian.top/gtqhmzzlfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtpqgflucv.html

[U70] PHP：PDO 事务
来源：http://hz.cqqwz.cn/gtjmfjsago.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.fzhhl.top/gtfilungjl.html

[U71] PHP：抛出异常
来源：http://hz.jqgfzy.top/gtruqcgozj.html

throw new RuntimeException("失败", 500);
来源：http://hz.aizwys.cn/gtkiosypen.html

[U72] PHP：写错误日志
来源：http://hz.shuidangran.top/gtrljfbppg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhixingplan.top/gtnehjwyvz.html

[U73] PHP：读取 ini 配置
来源：http://hz.yj20258.top/gtxhlbvaav.html

parse_ini_file("config.ini", true)
来源：http://hz.52xcode.cn/gtxvwfikrn.html

[U74] PHP：读取环境变量
来源：http://hz.hfpthk.cn/gtblzwoiwh.html

getenv("APP_ENV") ?: "production"
来源：http://hz.guowangkeji.top/gtkdimbibg.html

[U75] PHP：依赖注入
来源：http://hz.jinqigfzy.top/gtbmojqmqc.html

composer require psr/container
来源：http://hz.aizwys.cn/gtfkqfxhpm.html

[U76] PHP：简单路由
来源：http://hz.jlsjyb.cn/gtvyrmahqa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xziqi.cn/gtvngyeiti.html

[U77] PHP：模板渲染
来源：http://hz.jinqigufen.top/gtvemfmhlo.html

composer require twig/twig
来源：http://hz.0kj1m.cn/gtoszpcypu.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtxepigpxl.html

composer require --dev phpunit/phpunit
来源：http://hz.zhijiandao.cn/gtqwjopvow.html

[U79] PHP：静态分析
来源：http://hz.ivvv.top/gtpvygplfj.html

composer require --dev phpstan/phpstan
来源：http://hz.yj20258888.top/gtbuepbdpr.html

[U80] PHP：代码规范修复
来源：http://hz.pycfn.com/gtucpziits.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuanzx.com/gtwbjupajd.html

[U81] JS：初始化项目
来源：http://hz.zhiwuduotai.top/gthunnrsnx.html

npm init -y;  npm i express
来源：http://hz.jinyuanbaomall.cn/gtpwtzruvm.html

[U82] JS：package.json 脚本
来源：http://hz.chenzaomai.com/gtmnkaemyh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.nwbrower.top/gtqgplqupd.html

[U83] JS：ES Module 导入导出
来源：http://hz.ywan-chungtsiang.top/gtcopastje.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shangyingyoupin.top/gtsudzkldh.html

[U84] JS：CommonJS 写法
来源：http://hz.feifeiyinyue.top/gtsnwvgppn.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuanzhike.top/gtnbmsulua.html

[U85] JS：可选链
来源：http://hz.iojbl.cn/gtqpvrwqyq.html

a?.b?.c
来源：http://hz.jinqigufen.top/gtdwhwndxh.html

[U86] JS：空值合并
来源：http://hz.jqgufenzy.top/gtzlvrayeu.html

a ?? b
来源：http://hz.birdmap.top/gtegbkiunm.html

[U87] JS：解构默认值
来源：http://hz.vqdsnc.cn/gtnftlkkth.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hongshengwenyu.top/gtbsliejkv.html

[U88] JS：对象展开合并
来源：http://hz.jianghu66.top/gtqskjtxiz.html

{ ...a, ...b }
来源：http://hz.sweek.top/gtuflfrqvv.html

[U89] JS：数组去重
来源：http://hz.yuanzhike.top/gtuhkewbbr.html

[...new Set(arr)]
来源：http://hz.sweek.top/gtkyokqxig.html

[U90] JS：数字数组排序
来源：http://hz.hnxiangtu.top/gtegfbpytu.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtkvfhcune.html

[U91] JS：对象键值遍历
来源：http://hz.jianghu66.top/gtephouhqc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.ybcxt.top/gtxpdanxae.html

[U92] JS：深拷贝
来源：http://hz.shangyingyoupin.top/gtqfxyscap.html

structuredClone(obj)
来源：http://hz.xziqi.cn/gtweosffad.html

[U93] JS：模板字符串
来源：http://hz.sxryk.cn/gtysdccare.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtbcnbdpsp.html

[U94] JS：箭头函数
来源：http://hz.guannengcc.top/gtguyywqjg.html

const double = x => x * 2;
来源：http://hz.shanyushiyangkeji.top/gtdmvvjydg.html

[U95] JS：Promise 包装
来源：http://hz.cdnleiting.top/gttqanvicz.html

new Promise((resolve, reject) => {})
来源：http://hz.zhaomingkeji.xyz/gtpgatvxgn.html

[U96] JS：async/await 与异常
来源：http://hz.zycfv.cn/gtpogcadum.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtjzqotkmk.html

[U97] JS：并发请求
来源：http://hz.jinqigfzy.top/gtxgpsrepm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtwgsqnbyd.html

[U98] JS：fetch 带 JSON
来源：http://hz.bjfxy.top/gtusnryxuz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.0kj1m.cn/gtklrhbzui.html

[U99] JS：事件监听
来源：http://hz.fengsongda.top/gtjgstwxjt.html

el.addEventListener("click", e => {})
来源：http://hz.feifeiyinyue.top/gtsenlkxua.html

[U100] JS：DOM 查询
来源：http://hz.hywenlv.cn/gthpqidtlk.html

document.querySelector(".item")
来源：http://hz.shangyingyoupin.top/gtrotymqls.html

[U101] JS：classList 操作
来源：http://hz.shangyingyoupin.top/gtbqxedxfs.html

el.classList.toggle("active")
来源：http://hz.zhaomingkeji.xyz/gtuvczfivm.html

[U102] JS：本地存储
来源：http://hz.aibaodan.cn/gttpmtsxbf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.pengpengdd.cyou/gtrvrklsgw.html

[U103] JS：定时器
来源：http://hz.yvedp.cn/gtzwnjmyer.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jiagoushi.top/gtyljzoxyy.html

[U104] JS：防抖
来源：http://hz.sxryk.cn/gtimupfelx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtzwuongny.html

[U105] JS：节流
来源：http://hz.kuanghao11.cn/gtlbpcqljy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtdsigyhvz.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtetwyapxd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gteonszzqf.html

[U107] JS：数字千分位
来源：http://hz.nanxuanxn.top/gtacltofky.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.316326.xyz/gtmyhienhz.html

[U108] JS：随机整数
来源：http://hz.sxryk.cn/gtibzdjmid.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aibaodan.cn/gtmwxlfryo.html

[U109] JS：数组分组
来源：http://hz.guannengcc.top/gtmoyttqur.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtufiakdaq.html

[U110] JS：数组分块
来源：http://hz.jqgfzy.top/gtlfuhbwdf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gotoacloud.top/gtpdpnujve.html

[U111] JS：对象转 Map
来源：http://hz.wangshuangyany.cn/gtmstoikhi.html

new Map(Object.entries(obj))
来源：http://hz.gaohongyu789.top/gtbnsqlgng.html

[U112] JS：字符串补位
来源：http://hz.c1oappe.top/gtagzoudpe.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gteffxkita.html

[U113] JS：正则替换全部
来源：http://hz.zhiwuduotai.top/gtxhulpuxt.html

s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtovimnryz.html

[U114] JS：JSON 深比较
来源：http://hz.shangyingyoupin.top/gticvthcpx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtmofyooet.html

[U115] JS：生成 UUID
来源：http://hz.vqdsnc.cn/gtbfncebco.html

crypto.randomUUID()
来源：http://hz.sweek.top/gtygxamten.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jianghu66.top/gtuhyhswlb.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ppjwa.cn/gtmuyeizox.html

[U117] JS：单元测试
来源：http://hz.wangshuangyany.cn/gtecpalder.html

npm i -D vitest;  npx vitest
来源：http://hz.iojbl.cn/gtneqjyuqt.html

[U118] JS：开发服务器
来源：http://hz.yj20258.top/gtnshjotsw.html

npm i -D vite;  npx vite
来源：http://hz.jinqigfzy.top/gtcthalqrv.html

[U119] JS：生产构建
来源：http://hz.nanxuanxn.top/gtgirmztja.html

npx vite build
来源：http://hz.bjfxy.top/gtyomkzixz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hysaishi.cn/gtmrvthcbk.html

import.meta.env.VITE_API_URL
来源：http://hz.xuanzx.com/gtxxpflris.html

================================================================================
来源：http://hz.nwbrower.top/gtxfpxomyp.html

统计汇总
来源：http://hz.chenzaomai.com/gtkygjsuza.html

================================================================================
来源：http://hz.smart0.xyz/gtppryrmho.html

按语言统计（条）：
来源：http://hz.smart0.xyz/gtufzmwsnd.html

Python ......... 252
来源：http://hz.dashuyun.cn/gtgufiothb.html

PHP ............ 252
来源：http://hz.gzhubu.top/gtclfrcigv.html

JavaScript ..... 252
来源：http://hz.shangyingyoupin.top/gtggrgkons.html

TypeScript ..... 212
来源：http://hz.cqqwz.cn/gtfiuofmrd.html

Java ........... 212
来源：http://hz.jianghu66.top/gtuauojpoy.html

Go ............. 212
来源：http://hz.tian-w.cn/gtfatmbuyn.html

Ruby ........... 212
来源：http://hz.cheryme.top/gtbunzvrgd.html

C# ............. 212
来源：http://hz.tanke756.top/gtwfpnmdzl.html

C .............. 30
来源：http://hz.vqdsnc.cn/gturnbxdpj.html

C++ ............ 30
来源：http://hz.redwolf501.top/gtcaunxnuo.html

SQL ............ 90
来源：http://hz.nanxuanxn.top/gtxqqqvgvj.html

Bash ........... 80
来源：http://hz.zhongyouzk.top/gtzwdakdea.html

Kotlin ......... 15
来源：http://hz.mhx1999.top/gtgzpcgzit.html

Swift .......... 15
来源：http://hz.pycfn.com/gtzrsfgasr.html

Lua ............ 10
来源：http://hz.ydzc1.top/gtjiqpcgfv.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gtqrlxflio.html

Scala .......... 10
来源：http://hz.chenjidiqi.icu/gtjxnnksxy.html

------------------------------------
来源：http://hz.gaohongyu789.top/gtrzxchxlu.html

合计 ........... 2106 条
来源：http://hz.yongpay.top/gtqrqbonef.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtislnlyzj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hywenlv.cn/gtmtqbvsyi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhijiandao.cn/gtizruitwe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtenftrlco.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtzjzykdyx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.svipenyu.cn/gtnygywvpx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtmqrvqvke.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtvqfgqdfu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gtfyvtrnnr.html


<!-- 参考信息 -->