代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gthrgkdbma.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlyqxwoxy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sweek.top/gtvadgajgo.html

================================================================================
来源：http://hz.yangfankeji.com/gtagncpjzp.html

[U01] Py：创建虚拟环境
来源：http://hz.jqgufenzy.top/gtcfptzvqu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cucudq.cn/gtbbyecexg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gtuzipydcj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gtjtxzwdfk.html

[U03] Py：加载 .env 配置
来源：http://hz.9152youxi.cn/gtxgmtwohp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gogol.net.cn/gtekwihtcv.html

[U04] Py：变量调试打印
来源：http://hz.xylfe.cn/gtzbbqgixw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sysykeji.top/gtvsoahkxi.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtrbsdnofu.html

list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtiuardcfa.html

[U06] Py：合并两个字典
来源：http://hz.hysaishi.cn/gttmngvxxe.html

{**a, **b}
来源：http://hz.daria6918.cn/gtxazcipsd.html

[U07] Py：反转字典键值
来源：http://hz.hongshengwenyu.top/gttyqdfzdp.html

{v: k for k, v in d.items()}
来源：http://hz.yonumen.top/gthlqcetkv.html

[U08] Py：展平二维列表
来源：http://hz.zdqjudy.top/gtiuenhbou.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gtagitljpr.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtynjstssc.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gthhekaoqy.html

[U10] Py：按值排序字典
来源：http://hz.zhoulong.xyz/gtbrgrquoj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.svipenyu.cn/gtpbgeusku.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtpmwyglfv.html

(x * 2 for x in arr)
来源：http://hz.fzhhl.top/gtiqfbfjsa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guowangkeji.top/gtwdetybld.html

Counter(arr).most_common(3)
来源：http://hz.tanke756.top/gtsyutnzmd.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gthjiyttxc.html

deque(maxlen=10)
来源：http://hz.shuidangran.top/gtptwqlcdl.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258.top/gtavqjnbni.html

defaultdict(list)
来源：http://hz.birdmap.top/gtfrrxqrov.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtaliadrcx.html

t = time.perf_counter()
来源：http://hz.chenlongwang.top/gtxvqsfjjw.html

[U16] Py：命令行参数解析
来源：http://hz.zdqjudy.top/gtcpgwkxls.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sufxvd.cn/gtwivvwyiw.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtyvpxelws.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zdqjudy.top/gtvyeycbxe.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtzxwslkqw.html

pat = re.compile(r"\d+")
来源：http://hz.sweek.top/gtyeruamiz.html

[U19] Py：正则替换带回调
来源：http://hz.shanyushiyangtech.top/gtxpfafync.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtzkkqzofb.html

[U20] Py：缓存函数结果
来源：http://hz.kuanghao11.cn/gtxjlnsdyy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yongpay.top/gtjqdabzab.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gtwhvgcmku.html

@contextlib.contextmanager
来源：http://hz.ywan-chungtsiang.top/gtaqvggxxc.html

[U22] Py：矩阵转置
来源：http://hz.havefunace.top/gtxgfqpspl.html

list(zip(*m))
来源：http://hz.zhoulong.xyz/gtukfvohbi.html

[U23] Py：分块读取大文件
来源：http://hz.wangdashe.top/gtwxozzyoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinqigufen.top/gtpihoynck.html

[U24] Py：路径操作
来源：http://hz.chenzaomai.com/gtxlqtsbyo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.redwolf501.top/gtpzjfcils.html

[U25] Py：CSV 按字典读
来源：http://hz.guannengcc.top/gtlnsjvqod.html

csv.DictReader(f)
来源：http://hz.shzxlz.cn/gtxihrtgfh.html

[U26] Py：并发下载
来源：http://hz.zycfv.cn/gtfseacqpv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gtqcssekxv.html

[U27] Py：异步 HTTP
来源：http://hz.sxryk.cn/gtzgbaralo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zdqjudy.top/gtjkrazxpy.html

[U28] Py：类型别名
来源：http://hz.yangfankeji.com/gtuhbrvwkw.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtptxzvlie.html

[U29] Py：属性校验
来源：http://hz.cdnleiting.top/gtamcrqrhy.html

@property 与 @x.setter 配合
来源：http://hz.yj20258888.top/gtlcdlddgw.html

[U30] Py：数据类
来源：http://hz.xziqi.cn/gtcjwyxuax.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtvhmjyznf.html

[U31] Py：单测
来源：http://hz.tian-w.cn/gtqusdqyok.html

python -m pytest -q
来源：http://hz.ybcxt.top/gtcdhwqfsm.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gtpvhayzfe.html

ruff format . && ruff check --fix .
来源：http://hz.iojbl.cn/gtlkpqoehd.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gthciiiaow.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuanzhike.top/gtuvendrkj.html

[U34] Py：判断编码
来源：http://hz.jqgufenzy.top/gtubjmdetf.html

chardet.detect(raw)
来源：http://hz.xinyue.icu/gtnjffbvhn.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtddhocunk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxinkj.top/gteumujzsb.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtviipznag.html

schedule.every(10).minutes.do(job)
来源：http://hz.sufxvd.cn/gthmafmizh.html

[U37] Py：读写 Excel
来源：http://hz.jlsjyb.cn/gtsrhugotz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtxojlyuls.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtyzcxqeby.html

Path(__file__).resolve().parent
来源：http://hz.ppjwa.cn/gtzsxzcxhy.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinghuilouyu.cn/gtaxgelggp.html

sys.stdout.isatty()
来源：http://hz.zhoulong.xyz/gthndaxram.html

[U40] Py：打印到标准错误
来源：http://hz.gotoacloud.top/gtrfappbti.html

print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtfsohykza.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuanzhike.top/gtdeqpfpnh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gogol.net.cn/gtqlkpdcmq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yangfankeji.com/gthltlbors.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuanzhike.top/gtyqeiefsw.html

[U43] PHP：声明命名空间
来源：http://hz.xinyue.icu/gtuaucsflf.html

namespace App\Http;
来源：http://hz.wangshuangyany.cn/gtwanzpekw.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtbiyzvfmk.html

declare(strict_types=1);
来源：http://hz.zdqjudy.top/gtgribfnye.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yanxiufei.cn/gtmuwezrqm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtucamwsbs.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtulrnsycv.html

?string $name = null
来源：http://hz.quarkkingdee.top/gtdqhjqtwd.html

[U47] PHP：联合类型
来源：http://hz.zhongyouzk.top/gtsaqhggln.html

int|string $id
来源：http://hz.9152youxi.cn/gtsintuuby.html

[U48] PHP：纯枚举
来源：http://hz.gaohongyu789.top/gtfpyftqql.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yvedp.cn/gtmbyvsmns.html

[U49] PHP：只读属性
来源：http://hz.xuetiantiany.cn/gtbdcvhvbf.html

public readonly string $name
来源：http://hz.shuidangran.top/gtmwphisrs.html

[U50] PHP：构造器属性提升
来源：http://hz.feifeiyinyue.top/gtbvrwepwb.html

public function __construct(private int $id) {}
来源：http://hz.pengpengdd.cyou/gtajzgdiyp.html

[U51] PHP：数组解构
来源：http://hz.birdmap.top/gttpknfjad.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtbhtrtrdq.html

[U52] PHP：箭头函数
来源：http://hz.zhixingplan.top/gthytfkphz.html

$double = fn($x) => $x * 2;
来源：http://hz.hongshengwenyu.top/gtcenozgku.html

[U53] PHP：空合并运算符
来源：http://hz.fengsongda.top/gthkyxahid.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtlykgexfd.html

[U54] PHP：空安全调用
来源：http://hz.jinqigufen.top/gtwokdgnwy.html

$obj?->method()
来源：http://hz.ybcxt.top/gtzdrxcdal.html

[U55] PHP：match 表达式
来源：http://hz.zycfv.cn/gtovmtzdup.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nwbrower.top/gtiqpqqjaw.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtbupfmaae.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtnrvksdxp.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gtzvzoddqr.html

"值: {$a}"
来源：http://hz.cqqwz.cn/gtnyljftot.html

[U58] PHP：数组三件套
来源：http://hz.ivvv.top/gtvkeymoix.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gtkyuolmct.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtjxvjunaa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ehwqpu.com/gtbxyyumoq.html

[U60] PHP：JSON 编解码
来源：http://hz.iojbl.cn/gthltkmtmu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.0kj1m.cn/gtgndchjaa.html

[U61] PHP：正则
来源：http://hz.sxryk.cn/gtfpeqbhns.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtdabimotm.html

[U62] PHP：日期对象
来源：http://hz.yonumen.top/gtekiszsun.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtpinezjpw.html

[U63] PHP：文件读写
来源：http://hz.jinyuanbaomall.cn/gtbpzavsmt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shuidangran.top/gtumajfvfw.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtnedbkeez.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtlnvsvosv.html

[U65] PHP：会话
来源：http://hz.quarkkingdee.top/gtnvzodmga.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.0kj1m.cn/gtolpwgswk.html

[U66] PHP：设置 Cookie
来源：http://hz.zhengqikj.top/gtegoizdty.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jlsjyb.cn/gthqqwdtkt.html

[U67] PHP：处理文件上传
来源：http://hz.jinyuanbaomall.cn/gtqfklfphc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhijiandao.cn/gtogmnbtxt.html

[U68] PHP：PDO 连接
来源：http://hz.cdnleiting.top/gtaevsncmy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtzgnjkeft.html

[U69] PHP：PDO 预处理
来源：http://hz.xingfuxueyuan.xyz/gtxogfuvhz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dashuyun.cn/gtsowmsrlk.html

[U70] PHP：PDO 事务
来源：http://hz.hysaishi.cn/gtgaafebsx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258.top/gtqcvdfduj.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gtfxrhpfht.html

throw new RuntimeException("失败", 500);
来源：http://hz.cqqwz.cn/gtyouumwtq.html

[U72] PHP：写错误日志
来源：http://hz.xinyue.icu/gtzthxgzrg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cqqwz.cn/gtkfufmecd.html

[U73] PHP：读取 ini 配置
来源：http://hz.pengpengdd.cyou/gtjxrwpdvb.html

parse_ini_file("config.ini", true)
来源：http://hz.yonumen.top/gtxvnvuuhh.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtpkntrgte.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ywan-chungtsiang.top/gtlcxzhqvy.html

[U75] PHP：依赖注入
来源：http://hz.andypj.xyz/gtrxjfccyf.html

composer require psr/container
来源：http://hz.yanxiufei.cn/gtrffnhyun.html

[U76] PHP：简单路由
来源：http://hz.zdqjudy.top/gtphlzlhmq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.cdnleiting.top/gtzkxnrnjp.html

[U77] PHP：模板渲染
来源：http://hz.sxryk.cn/gtwauozzqq.html

composer require twig/twig
来源：http://hz.hysaishi.cn/gtkafracaq.html

[U78] PHP：单元测试
来源：http://hz.hnqzz.top/gtipvuiozu.html

composer require --dev phpunit/phpunit
来源：http://hz.wangshuangyany.cn/gtzpcifnjf.html

[U79] PHP：静态分析
来源：http://hz.smart0.xyz/gtjtnjejii.html

composer require --dev phpstan/phpstan
来源：http://hz.ehwqpu.com/gtasdpinly.html

[U80] PHP：代码规范修复
来源：http://hz.yanxiufei.cn/gtiooufiel.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtmhrnlgsl.html

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gtaxgwimwq.html

npm init -y;  npm i express
来源：http://hz.hnxiangtu.top/gtudtmnepz.html

[U82] JS：package.json 脚本
来源：http://hz.sweek.top/gtajfqkadu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.316326.xyz/gtctinarzm.html

[U83] JS：ES Module 导入导出
来源：http://hz.jinghuilouyu.cn/gtwoezpiax.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jianghu66.top/gtmvaflgra.html

[U84] JS：CommonJS 写法
来源：http://hz.hnxiangtu.top/gtodhkmbzs.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.316326.xyz/gtfnvcorca.html

[U85] JS：可选链
来源：http://hz.ydjk.org.cn/gtgqktzldg.html

a?.b?.c
来源：http://hz.ivvv.top/gtggwwqqfs.html

[U86] JS：空值合并
来源：http://hz.hammf.cn/gttybzylnj.html

a ?? b
来源：http://hz.jlsjyb.cn/gtmuuyclnd.html

[U87] JS：解构默认值
来源：http://hz.bjfxy.top/gtoltuznrp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yuxming.cn/gtmgcldfvq.html

[U88] JS：对象展开合并
来源：http://hz.fzhhl.top/gtzaduszku.html

{ ...a, ...b }
来源：http://hz.yonumen.top/gtxysjoxzh.html

[U89] JS：数组去重
来源：http://hz.vqdsnc.cn/gtqaasnsdv.html

[...new Set(arr)]
来源：http://hz.sweek.top/gtnqwmbsng.html

[U90] JS：数字数组排序
来源：http://hz.aibaodan.cn/gtolbmtolg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtbeitcwcu.html

[U91] JS：对象键值遍历
来源：http://hz.chenjidiqi.icu/gtarvgmjdh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cashguo.top/gtxfuiqrxm.html

[U92] JS：深拷贝
来源：http://hz.chenlongwang.top/gtrxkhbucb.html

structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtcjxfrolq.html

[U93] JS：模板字符串
来源：http://hz.nwbrower.top/gtrcwksivm.html

`共 ${n} 条`
来源：http://hz.smart0.xyz/gtxygqivwn.html

[U94] JS：箭头函数
来源：http://hz.tanke756.top/gtjqoopxda.html

const double = x => x * 2;
来源：http://hz.hnxiangtu.top/gtckwdluut.html

[U95] JS：Promise 包装
来源：http://hz.xinyue.icu/gtikigsysa.html

new Promise((resolve, reject) => {})
来源：http://hz.wangdashe.top/gtvpnrfcpm.html

[U96] JS：async/await 与异常
来源：http://hz.gaohongyu789.top/gtbonimczt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtjyrsrltg.html

[U97] JS：并发请求
来源：http://hz.chenlongwang.top/gthyweumzm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtjofuzrob.html

[U98] JS：fetch 带 JSON
来源：http://hz.havefunace.top/gtsetfivgb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ppjwa.cn/gtnoacikfs.html

[U99] JS：事件监听
来源：http://hz.xinyue.icu/gtndqbqcff.html

el.addEventListener("click", e => {})
来源：http://hz.tanke756.top/gtqcrwdiit.html

[U100] JS：DOM 查询
来源：http://hz.hnqzz.top/gtgmlrvfrw.html

document.querySelector(".item")
来源：http://hz.c1oappe.top/gtgygnkgpk.html

[U101] JS：classList 操作
来源：http://hz.aibaodan.cn/gtwxufmjzg.html

el.classList.toggle("active")
来源：http://hz.yueranfly.top/gthllnbhcy.html

[U102] JS：本地存储
来源：http://hz.yonumen.top/gtrpgetrxc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gtliuxorpd.html

[U103] JS：定时器
来源：http://hz.ehwqpu.com/gtmebufnph.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangtech.top/gtgrrxpmir.html

[U104] JS：防抖
来源：http://hz.chenlongwang.top/gtbhahzfcd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtkfvsnene.html

[U105] JS：节流
来源：http://hz.316326.xyz/gtjwxkqquq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.gotoacloud.top/gtfsqhmhkg.html

[U106] JS：日期格式化
来源：http://hz.cucudq.cn/gtlrzwcmcs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.tanke756.top/gtbsnukmgr.html

[U107] JS：数字千分位
来源：http://hz.gzhubu.top/gtlhvynqli.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.aibaodan.cn/gtfudfbobq.html

[U108] JS：随机整数
来源：http://hz.zhiwuduotai.top/gtfeasuylo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nwbrower.top/gtrnzseirw.html

[U109] JS：数组分组
来源：http://hz.sxryk.cn/gttrrlkaxz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtypjcpgfx.html

[U110] JS：数组分块
来源：http://hz.0kj1m.cn/gtzzwhfucn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.0kj1m.cn/gtpsaoynju.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gtiurjwiuq.html

new Map(Object.entries(obj))
来源：http://hz.birdmap.top/gtnsyfztmw.html

[U112] JS：字符串补位
来源：http://hz.aibaodan.cn/gtjzcmmdmr.html

"7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtteatywpf.html

[U113] JS：正则替换全部
来源：http://hz.redwolf501.top/gtathrgnkn.html

s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtvprbwdve.html

[U114] JS：JSON 深比较
来源：http://hz.yanxiufei.cn/gtxirkbesq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtvbklmlei.html

[U115] JS：生成 UUID
来源：http://hz.shanyushiyangtech.top/gtmgfvjxbw.html

crypto.randomUUID()
来源：http://hz.sweek.top/gthfhszfym.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cdnleiting.top/gtuzfrvzbu.html

/** @param {string} name */ function f(name) {}
来源：http://hz.dianchejie.cn/gtgxaafxjw.html

[U117] JS：单元测试
来源：http://hz.svipenyu.cn/gtijhwxpmi.html

npm i -D vitest;  npx vitest
来源：http://hz.tian-w.cn/gtljcmjylt.html

[U118] JS：开发服务器
来源：http://hz.yj202588.top/gtysyokgvi.html

npm i -D vite;  npx vite
来源：http://hz.cheryme.top/gtojlvnyxk.html

[U119] JS：生产构建
来源：http://hz.jinyuanbaomall.cn/gtedfrnvhb.html

npx vite build
来源：http://hz.daxiang520.top/gthixykuhl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhixingplan.top/gtryavvddy.html

import.meta.env.VITE_API_URL
来源：http://hz.yangfankeji.com/gtetckmbwx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzebifksz.html

统计汇总
来源：http://hz.gogol.net.cn/gtteeunmue.html

================================================================================
来源：http://hz.yueranfly.top/gtuluczlcf.html

按语言统计（条）：
来源：http://hz.fengsongda.top/gtfdzqwcpt.html

Python ......... 252
来源：http://hz.hnqzz.top/gtfvfsnaiz.html

PHP ............ 252
来源：http://hz.gaohongyu789.top/gtfeizzpim.html

JavaScript ..... 252
来源：http://hz.xingfuxueyuan.xyz/gteitehimd.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gtptilwnux.html

Java ........... 212
来源：http://hz.gaohongyu789.top/gtzmduuoxy.html

Go ............. 212
来源：http://hz.yvedp.cn/gtcipswmac.html

Ruby ........... 212
来源：http://hz.wangshuangyany.cn/gtewpkybfe.html

C# ............. 212
来源：http://hz.ybcxt.top/gtbbiuyetp.html

C .............. 30
来源：http://hz.fzhhl.top/gtnofrgbsm.html

C++ ............ 30
来源：http://hz.fzhhl.top/gtydozgxnx.html

SQL ............ 90
来源：http://hz.quarkkingdee.top/gteyxtxxfx.html

Bash ........... 80
来源：http://hz.shuidangran.top/gtcnpgfjoi.html

Kotlin ......... 15
来源：http://hz.wangshuangyany.cn/gtustphcyy.html

Swift .......... 15
来源：http://hz.zhijiandao.cn/gtvmxplmwv.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtkeeymyff.html

Perl ........... 10
来源：http://hz.kuanghao11.cn/gtbrfmcuml.html

Scala .......... 10
来源：http://hz.yj20258888.top/gthunuljcz.html

------------------------------------
来源：http://hz.52xcode.cn/gtvjryntsd.html

合计 ........... 2106 条
来源：http://hz.feifeiyinyue.top/gtscxjkvjg.html

按章节统计：
来源：http://hz.xuetiantiany.cn/gtjdecivme.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yj20258888.top/gtjtojmago.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtmvayzrdn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtkidnihxc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sxryk.cn/gtincxbwcz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ydzc1.top/gtefdgnelk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yanxiufei.cn/gtapcethuo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.tanke756.top/gteqfnfotj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.dianchejie.cn/gtgjdecjbj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtmsrgdgob.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jyoumei.cn/gteiwsinyk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtzkjcebog.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yongpay.top/gtylncijqq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gthtgvbqtn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hammf.cn/gtviidvpub.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhijiandao.cn/gtmkzyqkvd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.52xcode.cn/gtuvcicbqd.html

Q SQL 专题                              90
来源：http://hz.zhengqikj.top/gtgduijnoj.html

R Bash 专题                             80
来源：http://hz.xingfuxueyuan.xyz/gtoewlfaou.html

S C / C++ 专题                          60
来源：http://hz.hammf.cn/gtwbadunta.html

T 其他语言补充                          60
来源：http://hz.yongpay.top/gtcuhjadpx.html

U 高频实用片段                         120
来源：http://hz.0kj1m.cn/gtcvbdamgn.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtwuedwmhz.html

合计                                  2106 条
来源：http://hz.jianghu66.top/gteoueackk.html

--------------------------------------------------------------------------------
来源：http://hz.guannengcc.top/gtkjzdnsyy.html

使用提醒
来源：http://hz.fzhhl.top/gtndtcfgfx.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtbffeivtf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangdashe.top/gtwwbdamnp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hywenlv.cn/gtzmyjdzcf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yueranfly.top/gtqqipfixl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zycfv.cn/gtnhbyvowr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.316326.xyz/gtjgbkzrwm.html

—— 文件结束 ——
来源：http://hz.9152youxi.cn/gthzsbxemy.html


<!-- 参考信息 -->