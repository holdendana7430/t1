代发 wailian999

[U07] Py：反转字典键值
来源：http://hz.hysaishi.cn/gtlvbecybc.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtttrpmzwa.html

[U08] Py：展平二维列表
来源：http://hz.gaohongyu789.top/gtgxjoiade.html

[y for x in nested for y in x]
来源：http://hz.birdmap.top/gtanzlfaeq.html

[U09] Py：字典取最大值的键
来源：http://hz.guannengcc.top/gtsuutylax.html

max(d, key=d.get)
来源：http://hz.tian-w.cn/gtfkpqkszq.html

[U10] Py：按值排序字典
来源：http://hz.hammf.cn/gtttlqcewm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtubpqpcmn.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtnsqytwma.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtoijzbgfo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gtxzdzwlea.html

Counter(arr).most_common(3)
来源：http://hz.yonumen.top/gtumntzirt.html

[U13] Py：固定长度队列
来源：http://hz.jinqigufen.top/gtskwaurwv.html

deque(maxlen=10)
来源：http://hz.hammf.cn/gtqoykbndm.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtwwrdiqdd.html

defaultdict(list)
来源：http://hz.bjfxy.top/gtbssaiiph.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gtqfprmlxu.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtmomxbzng.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtabgxtkhu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtunqxugbv.html

[U17] Py：初始化日志
来源：http://hz.pengpengdd.cyou/gtldkyqbsd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtnpghyuek.html

[U18] Py：预编译正则
来源：http://hz.tianlin.xyz/gtrgdbtjex.html

pat = re.compile(r"\d+")
来源：http://hz.zycfv.cn/gtmrtlkpsz.html

[U19] Py：正则替换带回调
来源：http://hz.zhijiandao.cn/gtrfoykvgk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnxiangtu.top/gtezsdomae.html

[U20] Py：缓存函数结果
来源：http://hz.dashuyun.cn/gtjqyarmin.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhongyouzk.top/gtqduoebqf.html

[U21] Py：自定义上下文管理器
来源：http://hz.wangdashe.top/gtdxhifscz.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtcyseawfy.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtenfruhmm.html

list(zip(*m))
来源：http://hz.cheryme.top/gtyoliwjwh.html

[U23] Py：分块读取大文件
来源：http://hz.aizwys.cn/gtzyvsmpqe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zycfv.cn/gtbjlrhvvu.html

[U24] Py：路径操作
来源：http://hz.guannengcc.top/gtftiwbrsp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.aizwys.cn/gtbnxppauu.html

[U25] Py：CSV 按字典读
来源：http://hz.guannengcc.top/gtnyjoyfie.html

csv.DictReader(f)
来源：http://hz.feifeiyinyue.top/gtsxwjtfmq.html

[U26] Py：并发下载
来源：http://hz.zhiwuduotai.top/gtwluvixgi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gotoacloud.top/gtyvcmpbpr.html

[U27] Py：异步 HTTP
来源：http://hz.yangfankeji.com/gtfhplwqnt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tian-w.cn/gtiljrxszj.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtokbncucb.html

UserId = int
来源：http://hz.yuanzhike.top/gtxfalrwru.html

[U29] Py：属性校验
来源：http://hz.gogol.net.cn/gttepehwpp.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtjnondabl.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtqqlmwlwz.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtmyemibrx.html

[U31] Py：单测
来源：http://hz.sweek.top/gtxkoluxix.html

python -m pytest -q
来源：http://hz.pycfn.com/gtywypimle.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtenkgpvtt.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gttleijxqa.html

[U33] Py：打包发布
来源：http://hz.nanxuanxn.top/gtboppjukv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cqqwz.cn/gtgirpppmu.html

[U34] Py：判断编码
来源：http://hz.sysykeji.top/gtebqlfofd.html

chardet.detect(raw)
来源：http://hz.ehwqpu.com/gttpcmorrr.html

[U35] Py：发送邮件
来源：http://hz.gaohongyu789.top/gtjlhcstxw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fzhhl.top/gtuxzgfuww.html

[U36] Py：定时任务
来源：http://hz.redwolf501.top/gtqsvlmdxw.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgufenzy.top/gtlxmfiivb.html

[U37] Py：读写 Excel
来源：http://hz.wangdashe.top/gtlanahnuw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.snrcjt.cn/gtwqmigskf.html

[U38] Py：获取脚本所在目录
来源：http://hz.dianchejie.cn/gtiitfscka.html

Path(__file__).resolve().parent
来源：http://hz.gotoacloud.top/gtvcwzmzic.html

[U39] Py：判断是否在交互环境
来源：http://hz.sufxvd.cn/gtwemhnnyb.html

sys.stdout.isatty()
来源：http://hz.ehwqpu.com/gtergdbbym.html

[U40] Py：打印到标准错误
来源：http://hz.havefunace.top/gtsfwlikvc.html

print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtxtqhvvjg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jiagoushi.top/gtzyabsvfn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aibaodan.cn/gttkosvmbo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuetiantiany.cn/gtvjcedhgl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xziqi.cn/gtoilrbdpk.html

[U43] PHP：声明命名空间
来源：http://hz.hfpthk.cn/gtlqjjpadm.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtndgyopqp.html

[U44] PHP：开启严格类型
来源：http://hz.daria6918.cn/gtnfnhhipa.html

declare(strict_types=1);
来源：http://hz.gotoacloud.top/gtksaihvvb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtftnekziy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtlburuayv.html

[U46] PHP：可空类型
来源：http://hz.aibaodan.cn/gtrizefvgl.html

?string $name = null
来源：http://hz.iojbl.cn/gtqdrsobik.html

[U47] PHP：联合类型
来源：http://hz.shzxlz.cn/gtlxhicshs.html

int|string $id
来源：http://hz.nanxuanxn.top/gtzhmcnimh.html

[U48] PHP：纯枚举
来源：http://hz.cheryme.top/gtcsrxsvwz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gthmebnbmv.html

[U49] PHP：只读属性
来源：http://hz.jiagoushi.top/gtplceqwlp.html

public readonly string $name
来源：http://hz.nanxuanxn.top/gtdaleeard.html

[U50] PHP：构造器属性提升
来源：http://hz.cucudq.cn/gtyvtlhmee.html

public function __construct(private int $id) {}
来源：http://hz.daria6918.cn/gtteyvycgi.html

[U51] PHP：数组解构
来源：http://hz.zhengqikj.top/gtwggjlvrq.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtqmxpurcr.html

[U52] PHP：箭头函数
来源：http://hz.shuidangran.top/gtgorhvgsn.html

$double = fn($x) => $x * 2;
来源：http://hz.andypj.xyz/gtilzoqlyx.html

[U53] PHP：空合并运算符
来源：http://hz.9152youxi.cn/gtfphuismf.html

$v = $a ?? $b ?? "default";
来源：http://hz.yongpay.top/gteyiurcoi.html

[U54] PHP：空安全调用
来源：http://hz.hongshengwenyu.top/gtxhwscgaj.html

$obj?->method()
来源：http://hz.shanyushiyangkeji.top/gtipapkucl.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gtpinshrnb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hfpthk.cn/gtesytkyml.html

[U56] PHP：命名参数
来源：http://hz.wangshuangyany.cn/gtqsqkqitn.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtcipbbzon.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gteuwnlfmi.html

"值: {$a}"
来源：http://hz.shangyingyoupin.top/gtfedplifi.html

[U58] PHP：数组三件套
来源：http://hz.shanyushiyangtech.top/gtxtryetxc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.iojbl.cn/gtkgsqmiil.html

[U59] PHP：自定义排序
来源：http://hz.shangyingyoupin.top/gtsqyjwwss.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtdqapfmqu.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtgydxuneo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.iojbl.cn/gtlddmzlhs.html

[U61] PHP：正则
来源：http://hz.9152youxi.cn/gtczamlywl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtkgizchzw.html

[U62] PHP：日期对象
来源：http://hz.shuidangran.top/gtltuieutf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj20258888.top/gthhyrbnyu.html

[U63] PHP：文件读写
来源：http://hz.zdqjudy.top/gteowmfkps.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ivvv.top/gttzfeeier.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtskcyiulc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gtaysltwdo.html

[U65] PHP：会话
来源：http://hz.cucudq.cn/gthuavrlpa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sxryk.cn/gttcztytqc.html

[U66] PHP：设置 Cookie
来源：http://hz.vqdsnc.cn/gtclzuowtl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xziqi.cn/gtwcmhtemb.html

[U67] PHP：处理文件上传
来源：http://hz.jyoumei.cn/gtdbadfazt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gogol.net.cn/gtboeywqmp.html

[U68] PHP：PDO 连接
来源：http://hz.yanxiufei.cn/gtzxitybfo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jiagoushi.top/gtwkiqdksz.html

[U69] PHP：PDO 预处理
来源：http://hz.smart0.xyz/gtigntsjmr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.wangshuangyany.cn/gtfbtlosnc.html

[U70] PHP：PDO 事务
来源：http://hz.yuxming.cn/gthzyobwcl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.meibo888.top/gtvoxtfovh.html

[U71] PHP：抛出异常
来源：http://hz.jlsjyb.cn/gtiynyslww.html

throw new RuntimeException("失败", 500);
来源：http://hz.ybcxt.top/gtsdjadnbr.html

[U72] PHP：写错误日志
来源：http://hz.hysaishi.cn/gtvtbccryl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jinqigufen.top/gtlmgnkazm.html

[U73] PHP：读取 ini 配置
来源：http://hz.kuanghao11.cn/gtisfaxure.html

parse_ini_file("config.ini", true)
来源：http://hz.xziqi.cn/gtbtgqmgfw.html

[U74] PHP：读取环境变量
来源：http://hz.zhijiandao.cn/gtmjbrrmbo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jiagoushi.top/gtmtyidugy.html

[U75] PHP：依赖注入
来源：http://hz.zhijiandao.cn/gttohhmaex.html

composer require psr/container
来源：http://hz.yongpay.top/gtvusvruae.html

[U76] PHP：简单路由
来源：http://hz.ehwqpu.com/gtkgzepnau.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxuanxn.top/gtjhuoweig.html

[U77] PHP：模板渲染
来源：http://hz.gzhubu.top/gtdrqhbnfv.html

composer require twig/twig
来源：http://hz.chenjidiqi.icu/gtuouobxtr.html

[U78] PHP：单元测试
来源：http://hz.daria6918.cn/gtcztlggfk.html

composer require --dev phpunit/phpunit
来源：http://hz.hywenlv.cn/gtmnpbghyo.html

[U79] PHP：静态分析
来源：http://hz.sweek.top/gteixtgtee.html

composer require --dev phpstan/phpstan
来源：http://hz.shangyingyoupin.top/gtzlemxgfh.html

[U80] PHP：代码规范修复
来源：http://hz.zhixingplan.top/gtvquygeaf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xuetiantiany.cn/gtyibjcvqz.html

[U81] JS：初始化项目
来源：http://hz.yj20258.top/gtvmrxdrnd.html

npm init -y;  npm i express
来源：http://hz.shzxlz.cn/gtgcmybbpe.html

[U82] JS：package.json 脚本
来源：http://hz.zhaomingkeji.xyz/gtiexjkzxa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinghuilouyu.cn/gtqkuftggv.html

[U83] JS：ES Module 导入导出
来源：http://hz.guannengcc.top/gtbycrfsac.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yonumen.top/gtwjitruxh.html

[U84] JS：CommonJS 写法
来源：http://hz.ydjk.org.cn/gtjwecnnxc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.smart0.xyz/gtlmrnpkxf.html

[U85] JS：可选链
来源：http://hz.chenlongwang.top/gtfcvpsrjt.html

a?.b?.c
来源：http://hz.xziqi.cn/gtnhraaxtv.html

[U86] JS：空值合并
来源：http://hz.daxiang520.top/gtwhixrmef.html

a ?? b
来源：http://hz.chenjidiqi.icu/gtnooziylp.html

[U87] JS：解构默认值
来源：http://hz.dashuyun.cn/gtvhcscuih.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhongyouzk.top/gtelykihsd.html

[U88] JS：对象展开合并
来源：http://hz.quarkkingdee.top/gtoodsodox.html

{ ...a, ...b }
来源：http://hz.shzxlz.cn/gtadfdgxak.html

[U89] JS：数组去重
来源：http://hz.havefunace.top/gttwbgxzkq.html

[...new Set(arr)]
来源：http://hz.yvedp.cn/gtfxefirdo.html

[U90] JS：数字数组排序
来源：http://hz.yvedp.cn/gtcyxepycq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtfliylfhq.html

[U91] JS：对象键值遍历
来源：http://hz.guowangkeji.top/gtnqlavnbj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.dashuyun.cn/gtdszbsvyi.html

[U92] JS：深拷贝
来源：http://hz.hywenlv.cn/gtrpotlpxy.html

structuredClone(obj)
来源：http://hz.hfpthk.cn/gtkkoduqgq.html

[U93] JS：模板字符串
来源：http://hz.xziqi.cn/gtjbwfuzho.html

`共 ${n} 条`
来源：http://hz.ppjwa.cn/gtmtjyinee.html

[U94] JS：箭头函数
来源：http://hz.cashguo.top/gtefpbjjmy.html

const double = x => x * 2;
来源：http://hz.guannengcc.top/gtnigdniyr.html

[U95] JS：Promise 包装
来源：http://hz.c1oappe.top/gtabpyzukt.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtlbewllat.html

[U96] JS：async/await 与异常
来源：http://hz.nanxinkj.top/gtzgkkwfqs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtfxqxbiiv.html

[U97] JS：并发请求
来源：http://hz.fzhhl.top/gtfjdzvjwo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gthwmjaxmt.html

[U98] JS：fetch 带 JSON
来源：http://hz.snrcjt.cn/gtsfhjtcnq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.vqdsnc.cn/gtiiglgggn.html

[U99] JS：事件监听
来源：http://hz.yvedp.cn/gtnniukxxa.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gtfddeaiya.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtfbwlxbcd.html

document.querySelector(".item")
来源：http://hz.hysaishi.cn/gtvzdjqyvz.html

[U101] JS：classList 操作
来源：http://hz.ivvv.top/gtuleybbdh.html

el.classList.toggle("active")
来源：http://hz.xuetiantiany.cn/gtdpjfqcnn.html

[U102] JS：本地存储
来源：http://hz.jinqigfzy.top/gtctdripyx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tanke756.top/gtiknsfgho.html

[U103] JS：定时器
来源：http://hz.jinyuanbaomall.cn/gtcjlpgboa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.havefunace.top/gtlzfnrhec.html

[U104] JS：防抖
来源：http://hz.9152youxi.cn/gtcjlubfrq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tian-w.cn/gtgxdacyul.html

[U105] JS：节流
来源：http://hz.cucudq.cn/gtidnyvwyc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.pycfn.com/gttkvhnbap.html

[U106] JS：日期格式化
来源：http://hz.jianghu66.top/gtmvvhpobg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sweek.top/gtnbmjijlm.html

[U107] JS：数字千分位
来源：http://hz.yvedp.cn/gtfmxzcjcs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinqigufen.top/gtsgisylmn.html

[U108] JS：随机整数
来源：http://hz.wangshuangyany.cn/gtydqlxxzb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtabqniekv.html

[U109] JS：数组分组
来源：http://hz.jyoumei.cn/gtvubapkif.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtcqgpeqdn.html

[U110] JS：数组分块
来源：http://hz.feifeiyinyue.top/gtmfcwfslw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sufxvd.cn/gtgcgshpar.html

[U111] JS：对象转 Map
来源：http://hz.hammf.cn/gtjsmrwumy.html

new Map(Object.entries(obj))
来源：http://hz.iojbl.cn/gtlvjuguwy.html

[U112] JS：字符串补位
来源：http://hz.cashguo.top/gttzsoopfl.html

"7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtxigncdwf.html

[U113] JS：正则替换全部
来源：http://hz.redwolf501.top/gtlxgjxwha.html

s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtzvxodpjy.html

[U114] JS：JSON 深比较
来源：http://hz.gogol.net.cn/gtadcwqssa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtlyrqkepc.html

[U115] JS：生成 UUID
来源：http://hz.fzhhl.top/gtfdjwzcaj.html

crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtgsotuure.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tian-w.cn/gtzqmwcrmr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xuetiantiany.cn/gtffegdsml.html

[U117] JS：单元测试
来源：http://hz.hnxiangtu.top/gtrhjavpke.html

npm i -D vitest;  npx vitest
来源：http://hz.zhiwuduotai.top/gtqmlixruu.html

[U118] JS：开发服务器
来源：http://hz.hnxiangtu.top/gtlpaiebtm.html

npm i -D vite;  npx vite
来源：http://hz.andypj.xyz/gtrexzgfxr.html

[U119] JS：生产构建
来源：http://hz.xinyue.icu/gtpxmpjbad.html

npx vite build
来源：http://hz.sxryk.cn/gtgdezwfdm.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhaomingkeji.xyz/gtoruyzefo.html

import.meta.env.VITE_API_URL
来源：http://hz.quarkkingdee.top/gtkpffslcg.html

================================================================================
来源：http://hz.snrcjt.cn/gtxlktjjio.html

统计汇总
来源：http://hz.aibaodan.cn/gtvramjoli.html

================================================================================
来源：http://hz.zdqjudy.top/gtejybwrry.html

按语言统计（条）：
来源：http://hz.iojbl.cn/gtwbrkdsxf.html

Python ......... 252
来源：http://hz.0kj1m.cn/gtrbgzleol.html

PHP ............ 252
来源：http://hz.hnxiangtu.top/gtzvneoohi.html

JavaScript ..... 252
来源：http://hz.aizwys.cn/gtcztrbprh.html

TypeScript ..... 212
来源：http://hz.guannengcc.top/gtmitbhygc.html

Java ........... 212
来源：http://hz.xziqi.cn/gtleuigtyf.html

Go ............. 212
来源：http://hz.hongshengwenyu.top/gtblhgqaev.html

Ruby ........... 212
来源：http://hz.quarkkingdee.top/gtmotnovho.html

C# ............. 212
来源：http://hz.snrcjt.cn/gttgugnyle.html

C .............. 30
来源：http://hz.zdqjudy.top/gtzzvpwtkp.html

C++ ............ 30
来源：http://hz.jinghuilouyu.cn/gtdzcmxhig.html

SQL ............ 90
来源：http://hz.birdmap.top/gtxwypnitk.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtnakqzger.html

Kotlin ......... 15
来源：http://hz.pengpengdd.cyou/gtkjfbfwmi.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gtlacdgqdk.html

Lua ............ 10
来源：http://hz.chenjidiqi.icu/gtxnqerckx.html

Perl ........... 10
来源：http://hz.kuanghao11.cn/gtvjjbtqty.html

Scala .......... 10
来源：http://hz.shanyushiyangtech.top/gtbadbkjso.html

------------------------------------
来源：http://hz.316326.xyz/gtnchgncas.html

合计 ........... 2106 条
来源：http://hz.jyoumei.cn/gtrqeievfn.html

按章节统计：
来源：http://hz.zhaomingkeji.xyz/gtychhjyqw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.fengsongda.top/gtsoyubfjb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtzdnmgkyn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenjidiqi.icu/gtlfmqfyuy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.wangshuangyany.cn/gtcmnpotqz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zdqjudy.top/gthlxxfmxr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.quarkkingdee.top/gtbjvyyoyb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtbqawwras.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.shuidangran.top/gtossufjva.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtdqshithj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtvdgrqkjg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtwwuokbid.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yj20258.top/gtaxdczigz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtrxcfwnxe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtmvojhokd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sufxvd.cn/gtkmwcxfot.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ydjk.org.cn/gtzumkugmi.html

Q SQL 专题                              90
来源：http://hz.c1oappe.top/gtjxzuizlg.html

R Bash 专题                             80
来源：http://hz.nanxinkj.top/gtiswvqlhf.html

S C / C++ 专题                          60
来源：http://hz.xinyue.icu/gtwehgonci.html

T 其他语言补充                          60
来源：http://hz.cqqwz.cn/gtwuqqqevr.html

U 高频实用片段                         120
来源：http://hz.gaohongyu789.top/gtjptjwvta.html

------------------------------------
来源：http://hz.gzhubu.top/gtcuoxcpfs.html

合计                                  2106 条
来源：http://hz.hfpthk.cn/gtavfzhkxd.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtuuwekssm.html

使用提醒
来源：http://hz.ydjk.org.cn/gtxdcsxnej.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtcjffvohm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtcwadykbn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.0kj1m.cn/gtbhkdqxej.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gzhubu.top/gtucdzipjj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.0kj1m.cn/gtphydxfcl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.guowangkeji.top/gtruasxffq.html

—— 文件结束 ——
来源：http://hz.dianchejie.cn/gtcegcrjdg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxpxkszvf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gthbfezzmf.html

Common Programming Examples Cheat Book
来源：http://hz.zhoulong.xyz/gtmteeingb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmbqhyutj.html

【收录内容】
来源：http://hz.daria6918.cn/gtptgmyign.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hnqzz.top/gttlpwdeuy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yuxming.cn/gtoplgcgpo.html

SQL · Bash · C · C++
来源：http://hz.zdqjudy.top/gttuublqtn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.316326.xyz/gtgkjtxtnr.html

【使用说明】
来源：http://hz.yanxiufei.cn/gtyoobvevj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.daxiang520.top/gtiflusmco.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.feifeiyinyue.top/gtgzymtgni.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxinkj.top/gtrvyncucx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ppjwa.cn/gtptkaabag.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shzxlz.cn/gtsolmorcy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jlsjyb.cn/gtvroxutjs.html


<!-- 参考信息 -->