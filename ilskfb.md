代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gtcsalwawe.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gtagewioew.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sufxvd.cn/gtxtxgfzfg.html

[T56] Scala：样例类
来源：http://hz.zhijiandao.cn/gtqookyuhy.html

case class User(name: String, age: Int)
来源：http://hz.ydjk.org.cn/gtyuafdniw.html

[T57] Scala：模式匹配
来源：http://hz.zhengqikj.top/gtdywpqwqb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtwrupalfn.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtorvymbhh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtyshdjnrj.html

[T59] Scala：循环
来源：http://hz.fzhhl.top/gtptalqlrw.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtazumwllc.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gtoonkcesn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tanke756.top/gtdgqyjxlq.html

================================================================================
来源：http://hz.gogol.net.cn/gtfukltodo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gttuyuejym.html

================================================================================
来源：http://hz.jinqigfzy.top/gtchadfarp.html

[U01] Py：创建虚拟环境
来源：http://hz.iojbl.cn/gtqihaymsb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhiwuduotai.top/gtbripqerl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.52xcode.cn/gtwqlerqbi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gtftthvgjt.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtgiyolsoo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtuwrwazjx.html

[U04] Py：变量调试打印
来源：http://hz.birdmap.top/gtzgefjzbr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cucudq.cn/gtwbgbavgx.html

[U05] Py：列表去重且保序
来源：http://hz.ydjk.org.cn/gtstajqpfs.html

list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtudrrjdtl.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtaywwsjon.html

{**a, **b}
来源：http://hz.ydzc1.top/gtrynocbqr.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtbfxrbxei.html

{v: k for k, v in d.items()}
来源：http://hz.ehwqpu.com/gtfwqojzbl.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtdxfaqkps.html

[y for x in nested for y in x]
来源：http://hz.andypj.xyz/gtiwbwcvqa.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtetypccrd.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtcxtqsknh.html

[U10] Py：按值排序字典
来源：http://hz.chenjidiqi.icu/gtatukiuko.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtfgdaaebt.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtgtrujakr.html

(x * 2 for x in arr)
来源：http://hz.sweek.top/gtfjgnusbw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.redwolf501.top/gtyntjezpt.html

Counter(arr).most_common(3)
来源：http://hz.0kj1m.cn/gtwzqmqwen.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtetsatcqh.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtshgyaqbb.html

[U14] Py：分组收集到列表
来源：http://hz.zycfv.cn/gtlsdjkyoc.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gtcedczcem.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtvmskkhca.html

t = time.perf_counter()
来源：http://hz.ppjwa.cn/gtouwclbco.html

[U16] Py：命令行参数解析
来源：http://hz.cucudq.cn/gtvocwhloh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.wangshuangyany.cn/gtnyzrzqhv.html

[U17] Py：初始化日志
来源：http://hz.fengsongda.top/gtdzcdufnx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zycfv.cn/gtryguewqc.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtyhozresx.html

pat = re.compile(r"\d+")
来源：http://hz.yuxming.cn/gtytoloume.html

[U19] Py：正则替换带回调
来源：http://hz.yvedp.cn/gtjwohklfa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtrcxpxsvj.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtjdolgznc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tian-w.cn/gtmdwjyzoh.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigfzy.top/gttwgrbwha.html

@contextlib.contextmanager
来源：http://hz.yj20258888.top/gtcheizvji.html

[U22] Py：矩阵转置
来源：http://hz.hysaishi.cn/gtkondniwk.html

list(zip(*m))
来源：http://hz.shuidangran.top/gtccrddgyd.html

[U23] Py：分块读取大文件
来源：http://hz.ydzc1.top/gtknwifbma.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtdfbinvvv.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtzgepcfuf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtmzwocnis.html

[U25] Py：CSV 按字典读
来源：http://hz.chenlongwang.top/gtlnhsjpuh.html

csv.DictReader(f)
来源：http://hz.aizwys.cn/gtzarldpcf.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtgnonxmzk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aibaodan.cn/gtngcnegyu.html

[U27] Py：异步 HTTP
来源：http://hz.fengsongda.top/gtbnbemmql.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zycfv.cn/gtvzajfote.html

[U28] Py：类型别名
来源：http://hz.aizwys.cn/gturqlqble.html

UserId = int
来源：http://hz.sweek.top/gtbjkhvkhr.html

[U29] Py：属性校验
来源：http://hz.wangshuangyany.cn/gtyohvgztu.html

@property 与 @x.setter 配合
来源：http://hz.shzxlz.cn/gtidpuzisy.html

[U30] Py：数据类
来源：http://hz.svipenyu.cn/gtkygtkmqe.html

@dataclass(slots=True)
来源：http://hz.52xcode.cn/gtvbyedtzh.html

[U31] Py：单测
来源：http://hz.jinqigfzy.top/gtfloeniwe.html

python -m pytest -q
来源：http://hz.fzhhl.top/gtwcqmlvkl.html

[U32] Py：代码格式化
来源：http://hz.iojbl.cn/gtzxclmxnn.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtvgoxtrlw.html

[U33] Py：打包发布
来源：http://hz.yj202588.top/gtqmoixduv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yangfankeji.com/gtemtyknpk.html

[U34] Py：判断编码
来源：http://hz.yuxming.cn/gtqxndltcy.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtyjbbqgyb.html

[U35] Py：发送邮件
来源：http://hz.havefunace.top/gtntcacwaz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.316326.xyz/gtqycohtyz.html

[U36] Py：定时任务
来源：http://hz.jlsjyb.cn/gtixwxhfqn.html

schedule.every(10).minutes.do(job)
来源：http://hz.yanxiufei.cn/gtzzivfnku.html

[U37] Py：读写 Excel
来源：http://hz.sysykeji.top/gtipkjcvod.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.bjfxy.top/gtuqyxusws.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhiwuduotai.top/gtouimimnt.html

Path(__file__).resolve().parent
来源：http://hz.xinyue.icu/gtatkberrl.html

[U39] Py：判断是否在交互环境
来源：http://hz.gotoacloud.top/gtkojdenrf.html

sys.stdout.isatty()
来源：http://hz.xingfuxueyuan.xyz/gtroowmxrg.html

[U40] Py：打印到标准错误
来源：http://hz.fzhhl.top/gtcytpedru.html

print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gthrlixbft.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhaomingkeji.xyz/gtpznramte.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtxbggptje.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.daria6918.cn/gtfrxzxlyj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydzc1.top/gtvmtpowsj.html

[U43] PHP：声明命名空间
来源：http://hz.snrcjt.cn/gtzeawnnvk.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gthyjsbdpf.html

[U44] PHP：开启严格类型
来源：http://hz.fengsongda.top/gtwxaemkty.html

declare(strict_types=1);
来源：http://hz.9152youxi.cn/gtrkhvbpij.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydjk.org.cn/gtiewjsuve.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtowmrieyd.html

[U46] PHP：可空类型
来源：http://hz.sweek.top/gtckiqfyhk.html

?string $name = null
来源：http://hz.shzxlz.cn/gtlgefjcrx.html

[U47] PHP：联合类型
来源：http://hz.zhixingplan.top/gtthruteul.html

int|string $id
来源：http://hz.shuidangran.top/gtigdifxsf.html

[U48] PHP：纯枚举
来源：http://hz.yj20258.top/gtczoikvfu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yangfankeji.com/gtvwawprvy.html

[U49] PHP：只读属性
来源：http://hz.ybcxt.top/gtwmzoqtom.html

public readonly string $name
来源：http://hz.jinyuanbaomall.cn/gtmcxegxbg.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtnyvvobqr.html

public function __construct(private int $id) {}
来源：http://hz.pycfn.com/gtscnayeme.html

[U51] PHP：数组解构
来源：http://hz.hywenlv.cn/gtizvzrbip.html

[$a, $b] = $arr;
来源：http://hz.c1oappe.top/gtobeeiocu.html

[U52] PHP：箭头函数
来源：http://hz.daxiang520.top/gtqgapszdf.html

$double = fn($x) => $x * 2;
来源：http://hz.0kj1m.cn/gteudzjekw.html

[U53] PHP：空合并运算符
来源：http://hz.gaohongyu789.top/gtqvzhxvmh.html

$v = $a ?? $b ?? "default";
来源：http://hz.smart0.xyz/gtffkbxeqj.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gttajwzfdm.html

$obj?->method()
来源：http://hz.haohaochexian.top/gthhfhyxju.html

[U55] PHP：match 表达式
来源：http://hz.jinyuanbaomall.cn/gtgtxrmnfm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yanxiufei.cn/gtdflstyku.html

[U56] PHP：命名参数
来源：http://hz.ppjwa.cn/gtswaljrdr.html

f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtgqkjzdkp.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gthoicickx.html

"值: {$a}"
来源：http://hz.ywan-chungtsiang.top/gtlmyiqdnz.html

[U58] PHP：数组三件套
来源：http://hz.yj202588.top/gtbyzwiylk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtrolktyly.html

[U59] PHP：自定义排序
来源：http://hz.ppjwa.cn/gtydkouchn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ehwqpu.com/gtqwiytmfh.html

[U60] PHP：JSON 编解码
来源：http://hz.nanxuanxn.top/gtxoitvjed.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ywan-chungtsiang.top/gtzkhscpbt.html

[U61] PHP：正则
来源：http://hz.chenjidiqi.icu/gtcyxmtfia.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtdfhqsqqa.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gtibltncxq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigfzy.top/gtpzgipvit.html

[U63] PHP：文件读写
来源：http://hz.chenzaomai.com/gtffekrsyi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangkeji.top/gtuaybpkdt.html

[U64] PHP：目录遍历
来源：http://hz.jinyuanbaomall.cn/gtmxpnmvww.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hysaishi.cn/gtqxdfrvll.html

[U65] PHP：会话
来源：http://hz.haohaochexian.top/gtotssgwvl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yj202588.top/gtmspuoljc.html

[U66] PHP：设置 Cookie
来源：http://hz.jinghuilouyu.cn/gthjaxqoox.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhoulong.xyz/gtfdzervth.html

[U67] PHP：处理文件上传
来源：http://hz.yueranfly.top/gtybcfedfq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.xinyue.icu/gtxxoiwfzr.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gtcbogcvzd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.feifeiyinyue.top/gtrqnzmrzc.html

[U69] PHP：PDO 预处理
来源：http://hz.yj202588.top/gtutrojjqy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.svipenyu.cn/gtoruasntj.html

[U70] PHP：PDO 事务
来源：http://hz.yuxming.cn/gtluokmflr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenzaomai.com/gtvhxeiqap.html

[U71] PHP：抛出异常
来源：http://hz.fzhhl.top/gtrvipbqjp.html

throw new RuntimeException("失败", 500);
来源：http://hz.jiagoushi.top/gtpmosgnau.html

[U72] PHP：写错误日志
来源：http://hz.ppjwa.cn/gtzzbnvrjm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.quarkkingdee.top/gtlgqcrfsz.html

[U73] PHP：读取 ini 配置
来源：http://hz.wangdashe.top/gtjkdhmrfz.html

parse_ini_file("config.ini", true)
来源：http://hz.fengsongda.top/gtlzxuvvvf.html

[U74] PHP：读取环境变量
来源：http://hz.hammf.cn/gtgsppfcvz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xinyue.icu/gtfqynvxoy.html

[U75] PHP：依赖注入
来源：http://hz.shanyushiyangtech.top/gtyjvlzchd.html

composer require psr/container
来源：http://hz.shangyingyoupin.top/gtcpvrbtpo.html

[U76] PHP：简单路由
来源：http://hz.yangfankeji.com/gthlmtftjx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.wangshuangyany.cn/gtcorxdvip.html

[U77] PHP：模板渲染
来源：http://hz.tanke756.top/gtrdzdonfl.html

composer require twig/twig
来源：http://hz.feifeiyinyue.top/gtbtgvfgkf.html

[U78] PHP：单元测试
来源：http://hz.hammf.cn/gtfuhqmyuq.html

composer require --dev phpunit/phpunit
来源：http://hz.yongpay.top/gtrgzcouim.html

[U79] PHP：静态分析
来源：http://hz.svipenyu.cn/gtokonerfq.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtnpiljxal.html

[U80] PHP：代码规范修复
来源：http://hz.zhongyouzk.top/gtyrsbwqdz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.yj20258888.top/gtzjfimqyx.html

[U81] JS：初始化项目
来源：http://hz.zhoulong.xyz/gtyucfjuym.html

npm init -y;  npm i express
来源：http://hz.wangdashe.top/gtshkrvzbk.html

[U82] JS：package.json 脚本
来源：http://hz.shanyushiyangtech.top/gtnsakvejq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.gaohongyu789.top/gtccwjoitd.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhiwuduotai.top/gtkfwkpbou.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.feifeiyinyue.top/gtockufbku.html

[U84] JS：CommonJS 写法
来源：http://hz.yj20258888.top/gttqrpvggh.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zhengqikj.top/gtzxtlpmwx.html

[U85] JS：可选链
来源：http://hz.ehwqpu.com/gtmxovhnlf.html

a?.b?.c
来源：http://hz.xziqi.cn/gtnrqoowxp.html

[U86] JS：空值合并
来源：http://hz.chenlongwang.top/gtyfodjort.html

a ?? b
来源：http://hz.shzxlz.cn/gtavstnbpy.html

[U87] JS：解构默认值
来源：http://hz.ybcxt.top/gtoztjtowh.html

const { a = 1, b = 2 } = obj;
来源：http://hz.yueranfly.top/gtqijuousd.html

[U88] JS：对象展开合并
来源：http://hz.hnxiangtu.top/gtgidcrueb.html

{ ...a, ...b }
来源：http://hz.yj20258.top/gtaissvjsb.html

[U89] JS：数组去重
来源：http://hz.ppjwa.cn/gtmzlwtmsa.html

[...new Set(arr)]
来源：http://hz.wangdashe.top/gthokepkfm.html

[U90] JS：数字数组排序
来源：http://hz.feifeiyinyue.top/gtuwwttqsd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtrssgfrnz.html

[U91] JS：对象键值遍历
来源：http://hz.redwolf501.top/gtfoepdmiv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.zhiwuduotai.top/gtfjiwvlbe.html

[U92] JS：深拷贝
来源：http://hz.mhx1999.top/gtsqwvazqq.html

structuredClone(obj)
来源：http://hz.aizwys.cn/gtstuyctyo.html

[U93] JS：模板字符串
来源：http://hz.dianchejie.cn/gtihglbfzv.html

`共 ${n} 条`
来源：http://hz.yj20258.top/gtooqbpanx.html

[U94] JS：箭头函数
来源：http://hz.yj202588.top/gtfzqzypma.html

const double = x => x * 2;
来源：http://hz.daxiang520.top/gtveuvrdpu.html

[U95] JS：Promise 包装
来源：http://hz.sufxvd.cn/gthakdyfdq.html

new Promise((resolve, reject) => {})
来源：http://hz.shanyushiyangtech.top/gtzpbwsoqr.html

[U96] JS：async/await 与异常
来源：http://hz.nanxuanxn.top/gtgzdbyfjk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtabyatada.html

[U97] JS：并发请求
来源：http://hz.jinyuanbaomall.cn/gtioblwfwn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtskuqwikd.html

[U98] JS：fetch 带 JSON
来源：http://hz.0kj1m.cn/gtdbjktqeh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.kuanghao11.cn/gtuuwohkag.html

[U99] JS：事件监听
来源：http://hz.feifeiyinyue.top/gtxszpyhyh.html

el.addEventListener("click", e => {})
来源：http://hz.smart0.xyz/gtmqhycqah.html

[U100] JS：DOM 查询
来源：http://hz.shangyingyoupin.top/gtzvrlzult.html

document.querySelector(".item")
来源：http://hz.316326.xyz/gteaotddud.html

[U101] JS：classList 操作
来源：http://hz.cheryme.top/gtubcqtdrf.html

el.classList.toggle("active")
来源：http://hz.havefunace.top/gtjkpvrmta.html

[U102] JS：本地存储
来源：http://hz.xuanzx.com/gtgullhapb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gthxecbhyl.html

[U103] JS：定时器
来源：http://hz.jianghu66.top/gtvqwizhri.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtdipscapm.html

[U104] JS：防抖
来源：http://hz.haohaochexian.top/gtmrpericn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtzndvzegq.html

[U105] JS：节流
来源：http://hz.nanxinkj.top/gtdahhutde.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yuanzhike.top/gtrhradvtx.html

[U106] JS：日期格式化
来源：http://hz.iojbl.cn/gtcvjgawxr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ivvv.top/gtlptzdkfw.html

[U107] JS：数字千分位
来源：http://hz.redwolf501.top/gttjpmepyd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.daxiang520.top/gtnkvsjirk.html

[U108] JS：随机整数
来源：http://hz.daxiang520.top/gtlqojppyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sxryk.cn/gtykptwlwa.html

[U109] JS：数组分组
来源：http://hz.gzhubu.top/gtmchgdyav.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtjczdgplz.html

[U110] JS：数组分块
来源：http://hz.snrcjt.cn/gthithdgme.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yj20258.top/gtzjfeyaxm.html

[U111] JS：对象转 Map
来源：http://hz.ehwqpu.com/gtacargipo.html

new Map(Object.entries(obj))
来源：http://hz.andypj.xyz/gthegslnww.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtyuznebuk.html

"7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtlqdhdadm.html

[U113] JS：正则替换全部
来源：http://hz.hongshengwenyu.top/gtesagivjg.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtxknagwiu.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtdcghmmzj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xylfe.cn/gtixjqqlon.html

[U115] JS：生成 UUID
来源：http://hz.chenlongwang.top/gtjbsijykn.html

crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtrqiqmcil.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxinkj.top/gtvejmnjtf.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj20258888.top/gtqjlnawkh.html

[U117] JS：单元测试
来源：http://hz.guannengcc.top/gtiplwzjja.html

npm i -D vitest;  npx vitest
来源：http://hz.ydjk.org.cn/gtvjxcnohn.html

[U118] JS：开发服务器
来源：http://hz.yuxming.cn/gtmcjkxgzg.html

npm i -D vite;  npx vite
来源：http://hz.birdmap.top/gtvayoujik.html

[U119] JS：生产构建
来源：http://hz.smart0.xyz/gtrserabzm.html

npx vite build
来源：http://hz.shanyushiyangkeji.top/gtiuurzvgf.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.haohaochexian.top/gtjurplcka.html

import.meta.env.VITE_API_URL
来源：http://hz.yueranfly.top/gtjpnfvdui.html

================================================================================
来源：http://hz.yuanzhike.top/gtvfoywoag.html

统计汇总
来源：http://hz.ydjk.org.cn/gtnnxotowf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttxgqhmqx.html

按语言统计（条）：
来源：http://hz.pengpengdd.cyou/gtjacidhem.html

Python ......... 252
来源：http://hz.shangyingyoupin.top/gtyjjwjsna.html

PHP ............ 252
来源：http://hz.hysaishi.cn/gtnngjgblv.html

JavaScript ..... 252
来源：http://hz.yueranfly.top/gtllxncjqz.html

TypeScript ..... 212
来源：http://hz.ehwqpu.com/gtqujaobxg.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtwvugjedk.html

Go ............. 212
来源：http://hz.zhoulong.xyz/gtfbacsyda.html

Ruby ........... 212
来源：http://hz.zhaomingkeji.xyz/gttrsawjkj.html

C# ............. 212
来源：http://hz.chenzaomai.com/gtbgffwpwi.html

C .............. 30
来源：http://hz.nwbrower.top/gtvxpudcgj.html

C++ ............ 30
来源：http://hz.jinyuanbaomall.cn/gtwhaszjye.html

SQL ............ 90
来源：http://hz.chenjidiqi.icu/gtevnysztw.html

Bash ........... 80
来源：http://hz.ppjwa.cn/gtwhbheuyo.html

Kotlin ......... 15
来源：http://hz.shzxlz.cn/gtkvvkthpm.html

Swift .......... 15
来源：http://hz.tianlin.xyz/gttjxkuooi.html

Lua ............ 10
来源：http://hz.gaohongyu789.top/gtnvzfxewv.html

Perl ........... 10
来源：http://hz.aibaodan.cn/gtccrsjnkj.html

Scala .......... 10
来源：http://hz.chenlongwang.top/gtmvrtbcby.html

------------------------------------
来源：http://hz.0kj1m.cn/gtwsfqzkso.html

合计 ........... 2106 条
来源：http://hz.hammf.cn/gtsnqxjrbj.html

按章节统计：
来源：http://hz.tian-w.cn/gtxqbsatyn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daria6918.cn/gtgurnbvyz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.tian-w.cn/gtooyhyxtk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gotoacloud.top/gtyrthjefc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hysaishi.cn/gtwesihdpm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnqzz.top/gtzxtnbkrm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtekybqqny.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ehwqpu.com/gtvkeiiglc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhiwuduotai.top/gtwgxuxusi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtjmxvefcb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ehwqpu.com/gtypvtrxie.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtlecgynbh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yueranfly.top/gtwizwnsyc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gtddykgplx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtoomfiyis.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.hongshengwenyu.top/gtttyjqtfb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.snrcjt.cn/gtjqgpmshq.html

Q SQL 专题                              90
来源：http://hz.jqgufenzy.top/gtbfpehwxu.html

R Bash 专题                             80
来源：http://hz.kuanghao11.cn/gtskmgicbu.html

S C / C++ 专题                          60
来源：http://hz.bjfxy.top/gthvsjgywk.html

T 其他语言补充                          60
来源：http://hz.sweek.top/gttuuourcz.html


<!-- 参考信息 -->