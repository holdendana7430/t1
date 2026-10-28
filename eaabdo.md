代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtejfqxtjh.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtypxlecgu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtcxxjbmfk.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtysjkxkzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aibaodan.cn/gtjleeooja.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gticndkspg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtnihsujuz.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtldhaejzc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtvmmeyxyu.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtiggpssry.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhijiandao.cn/gtkwxpmyvm.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtiypfgdci.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtodcaqlsf.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtjfewlbvt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydzc1.top/gttabczjkn.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtuiiofmcg.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gtynystcak.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtavwjoyir.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtyavmhkqu.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtmhlhpfbi.html

cmd >/dev/null 2>&1
来源：http://hz.feifeiyinyue.top/gtjzpcrryj.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtkvkfzrxl.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtstjjeozo.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtxclicbyx.html

find . -name "*.log" -type f
来源：http://hz.cdnleiting.top/gtvwaqtnbs.html

[R44] 按修改时间查找
来源：http://hz.zdqjudy.top/gtantzshxe.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtwsmylcws.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtnjoarhfi.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gthbqbdbvh.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtxcsyeufd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtngujvoik.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtvuncdoav.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtqwzmcecm.html

[R48] awk 取指定列
来源：http://hz.dashuyun.cn/gtvvlwkgzu.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtolrcebdf.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtzkggxcfg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.havefunace.top/gtuavwxcyk.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtzyqnacqo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtwbsscdpl.html

[R51] 排序去重取前几
来源：http://hz.cheryme.top/gtycnbyddg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtchohydeh.html

[R52] 统计行数
来源：http://hz.ywan-chungtsiang.top/gtmpdgkjya.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtpdevxrhf.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gttyefzoal.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.c1oappe.top/gtplcdoayp.html

[R54] 比较两个文件
来源：http://hz.tian-w.cn/gtpctafidl.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtgxbzttws.html

[R55] 压缩与解压
来源：http://hz.ppjwa.cn/gtsedyefvb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gtivgdkhro.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtgzbhisgq.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtgghsmwpv.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtfenwtplw.html

ssh user@host 'uptime'
来源：http://hz.jqgufenzy.top/gtloewshhg.html

[R58] 下载文件
来源：http://hz.smart0.xyz/gtkpmovhui.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtljubspga.html

[R59] 发 POST JSON
来源：http://hz.smart0.xyz/gtagihmrru.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtxdfziaqv.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gtccbarihd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtdpnzapbd.html

[R61] 磁盘占用
来源：http://hz.ybcxt.top/gtqqijlrac.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtgcpjrwmp.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtjbkirjrz.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gtwibprviq.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtpnioykda.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtyyipxizg.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtyqcrqfnl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtimpdxshv.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gtoseboqej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtweobfzcy.html

[R66] 定时任务
来源：http://hz.cucudq.cn/gtlsbbrpoh.html

crontab -e;  crontab -l
来源：http://hz.ybcxt.top/gtvgngjmwu.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtcufuoaed.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtprjethuz.html

[R68] 计算文件校验值
来源：http://hz.smart0.xyz/gtwukonqib.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuxming.cn/gtaspgszim.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gtsefrfaft.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtquwmnbop.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtxgmlckoz.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gtgvxrbjko.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtatcnzhty.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtfjcwjudy.html

[R72] 等待端口就绪
来源：http://hz.dashuyun.cn/gtyjnzfmtn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtgtxbtnej.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gthtxefzop.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtdjokuapi.html

[R74] 批量重命名
来源：http://hz.nwbrower.top/gtjkyqbgse.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtvfkdvxpd.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtzwmjnzex.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtqtghhcac.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtwcrxowgx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtnzsgmhmt.html

[R77] 读取用户输入
来源：http://hz.sysykeji.top/gtuzwupadx.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtmzyzgkcv.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtprhtfqzl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hfpthk.cn/gtoetliueh.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtnmkvqbnl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daria6918.cn/gtabojuqqh.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gtrrovixbg.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtzzugkqov.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnnuxvwrp.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtnpwglxpg.html

================================================================================
来源：http://hz.9152youxi.cn/gtetmbcmaf.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtawekkzde.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtkhqzikqh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gthzfsloca.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gtzfzhefaf.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtswivquom.html

[S03] C：读入整数
来源：http://hz.jyoumei.cn/gtkxqpjedg.html

int x; scanf("%d", &x);
来源：http://hz.yj20258.top/gtgijtbots.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtfbqxovxb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtxnfmuooo.html

[S05] C：字符串长度
来源：http://hz.cucudq.cn/gtrabpawou.html

strlen(s)
来源：http://hz.tianlin.xyz/gtiswszjre.html

[S06] C：字符串比较
来源：http://hz.tanke756.top/gtspinoxqd.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtlbiamswc.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gttowwwweo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtakasqacb.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtvsadotqa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtdunhquzv.html

[S09] C：结构体定义与初始化
来源：http://hz.havefunace.top/gtbjorzmim.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtjguufxid.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtfvfmfvfh.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtlwjrldvv.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtkfwpuxhy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtkfszmqbc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xinyue.icu/gtnaygfmle.html

fclose(f);
来源：http://hz.tianlin.xyz/gtgtwspizn.html

[S12] C：写文件
来源：http://hz.aizwys.cn/gtxiznaads.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigfzy.top/gtsbzyypdm.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtggwqbdxs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ywan-chungtsiang.top/gtkpcnxzyt.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtwjoncnfj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtqkgasvml.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtuscnrxbt.html

(double) a / b
来源：http://hz.hysaishi.cn/gtkjulvcpp.html

[S16] C：位操作置位
来源：http://hz.jqgfzy.top/gtowsonqiv.html

x |= (1 << 3);
来源：http://hz.shangyingyoupin.top/gtmzqmxikt.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtzalmmaqq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtfverkaih.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtbmbcixut.html

int main(int argc, char **argv)
来源：http://hz.daria6918.cn/gtiklzprml.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtevtuvahp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtrrlkhmfk.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtehpzsjuo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtjvpuqzdd.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtghqtumbx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtbinvytqh.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtlbxzavmz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.birdmap.top/gtinxtoybl.html

[S23] C：随机数
来源：http://hz.chenjidiqi.icu/gtjamjmqoh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtpvkqzekp.html

[S24] C：获取本地时间
来源：http://hz.daxiang520.top/gtewzzfaui.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gogol.net.cn/gtpfqfzyru.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtysxfxfzf.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtprxtgrzu.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gttxamzaqc.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtuuuhgsmq.html

[S27] C：定义常量
来源：http://hz.shanyushiyangtech.top/gtzyaoicqp.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtgpxmueoo.html

[S28] C：静态变量
来源：http://hz.bjfxy.top/gtlytxdysh.html

static int counter = 0;
来源：http://hz.sufxvd.cn/gtrupmitkw.html

[S29] C：变参函数
来源：http://hz.pycfn.com/gtzvjtssvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtegczogil.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtmacamnhy.html

#ifndef X_H
来源：http://hz.jqgufenzy.top/gtcliztpah.html

#define X_H
来源：http://hz.jqgfzy.top/gtfofjamrg.html

#endif
来源：http://hz.jqgfzy.top/gtwkeyodcc.html

[S31] C++：Hello World
来源：http://hz.redwolf501.top/gtxzzncnfw.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtbhdqwlzd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtmkywddnc.html

[S32] C++：字符串
来源：http://hz.9152youxi.cn/gtukzyudhk.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtnfyrjovb.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtaguxogvr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtbdsqhida.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gthatiycog.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ppjwa.cn/gtryjwhkwg.html

[S35] C++：map
来源：http://hz.cdnleiting.top/gtjpiqfqtr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sysykeji.top/gtgwhzrhia.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtssuyxvgv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtimqxnlbz.html

[S37] C++：set
来源：http://hz.redwolf501.top/gthidfnrch.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtufvoxwhj.html

[S38] C++：排序
来源：http://hz.cucudq.cn/gtsvzzrkyp.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtuacsereu.html

[S39] C++：自定义比较器排序
来源：http://hz.guowangkeji.top/gtnledzepz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daria6918.cn/gtxlrdszyt.html

[S40] C++：查找元素
来源：http://hz.chenzaomai.com/gthabbtnah.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtpzityhua.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtxtfltafl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtimstynot.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtqpmtzcyu.html

class B : public Base { public: void f() override {} };
来源：http://hz.tianlin.xyz/gtsbgeaern.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtndrumnln.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gthcdevxdq.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gthpyrxicj.html

void inc(int &x) { ++x; }
来源：http://hz.yj20258888.top/gtkahoblfp.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gtyawahzky.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtxxtyjekq.html

[S46] C++：函数模板
来源：http://hz.meibo888.top/gtorxhsyuq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.bjfxy.top/gtwclisrgw.html

[S47] C++：结构化绑定遍历
来源：http://hz.bjfxy.top/gtatvhfapk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.birdmap.top/gtbyynerii.html

[S48] C++：逐行读文件
来源：http://hz.guannengcc.top/gtkbzpjnym.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtaxpijhyf.html

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gtfuqrxafp.html

[S49] C++：写文件
来源：http://hz.chenlongwang.top/gtbgcpamga.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtftthcvls.html

[S50] C++：格式化数字
来源：http://hz.wangshuangyany.cn/gtsksbulam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenjidiqi.icu/gttlupayju.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtriqdopay.html

static_cast<double>(a) / b
来源：http://hz.yanxiufei.cn/gtzbnzzdsf.html

[S52] C++：const 与 noexcept
来源：http://hz.chenlongwang.top/gtzcfuvaxl.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtgjpoqhgc.html

[S53] C++：移动语义
来源：http://hz.ehwqpu.com/gthdxjyuun.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gtkdhxuszr.html

[S54] C++：异常处理
来源：http://hz.9152youxi.cn/gtrxewtvon.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tianlin.xyz/gtonuxxirj.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gteaxvgjyk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtzbbtkwbj.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtdlwiyfxi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hammf.cn/gtlbassiqg.html

[S57] C++：编译期常量
来源：http://hz.jlsjyb.cn/gtfzdtjamh.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gttvsornln.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtvdhiwfrl.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtszqktykm.html

[S59] C++：静态断言
来源：http://hz.cqqwz.cn/gtybcidqyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtcgoqhjui.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtcqxxfovx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ppjwa.cn/gtvysbbhtk.html

================================================================================
来源：http://hz.jqgufenzy.top/gtezuojsah.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tianlin.xyz/gtrsuvfzof.html

================================================================================
来源：http://hz.xuanzx.com/gtbwxizlso.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtijwrcpng.html

println("Hello")
来源：http://hz.sweek.top/gtnkyeeszb.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtnuhiuhgm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtbztmnlxr.html

[T03] Kotlin：字符串模板
来源：http://hz.ybcxt.top/gtigteowvu.html

"值: $b"
来源：http://hz.yangfankeji.com/gthcccofsf.html

[T04] Kotlin：空安全
来源：http://hz.cdnleiting.top/gtlfcykkhu.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtkyokkofp.html

[T05] Kotlin：when 表达式
来源：http://hz.svipenyu.cn/gtalrsssdu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shangyingyoupin.top/gtsvtjufis.html

[T06] Kotlin：集合映射
来源：http://hz.iojbl.cn/gtxqeqkauz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtlyenodrx.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtimticsii.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtxmvtzbvw.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gthwdelpol.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtfzloreud.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtiirvkoru.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gtmveqxbga.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtajibrpcq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.birdmap.top/gtomzkcncl.html

[T11] Kotlin：协程
来源：http://hz.sysykeji.top/gtnmdwnygi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtoerathsc.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtsnoexxqi.html

val (a, b) = Pair(1, 2)
来源：http://hz.gzhubu.top/gtdeczijfe.html

[T13] Kotlin：只读 Map
来源：http://hz.hfpthk.cn/gtumupmhdt.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtdnuployz.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtthcsznvc.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtiakomqcr.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtwohqdahc.html

interface Shape { fun area(): Double }
来源：http://hz.birdmap.top/gtfffmdvpl.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangkeji.top/gtkrpbdclw.html

print("Hello")
来源：http://hz.zycfv.cn/gtantfwjsq.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtnbyvfkax.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtrbxoawvb.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtywbmscrn.html

"值: \(b)"
来源：http://hz.zycfv.cn/gtgxnirqsi.html

[T19] Swift：可选绑定
来源：http://hz.gogol.net.cn/gtbapkaisa.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtanhdkpes.html

[T20] Swift：数组操作
来源：http://hz.chenzaomai.com/gtuzrmptvt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guannengcc.top/gtocrmsjne.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gtjmtzdqcc.html

for x in a { print(x) }
来源：http://hz.jlsjyb.cn/gtrawycqyq.html

[T22] Swift：字典
来源：http://hz.sysykeji.top/gtwxoywezt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aibaodan.cn/gtqlwftapx.html

[T23] Swift：函数
来源：http://hz.sxryk.cn/gtxoyrooet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nwbrower.top/gttqkxbyoj.html

[T24] Swift：闭包
来源：http://hz.pycfn.com/gtzspvimih.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtlgyekqzc.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtjiobddhn.html

struct P { var x: Int }
来源：http://hz.shanyushiyangtech.top/gteldsqoox.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtvtlcazmw.html

class A: Base { override func f() {} }
来源：http://hz.haohaochexian.top/gtxzqrwwpx.html

[T27] Swift：错误处理
来源：http://hz.gogol.net.cn/gtlcyzxfnu.html

do { try f() } catch { print(error) }
来源：http://hz.316326.xyz/gteyaxuykl.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtlzgwndyc.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gtkzhbyuxs.html

[T29] Swift：guard 提前返回
来源：http://hz.aibaodan.cn/gtoppyancx.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtuklntquy.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtyzjtdjgc.html

protocol Shape { func area() -> Double }
来源：http://hz.ydzc1.top/gthocfgbqg.html

[T31] Lua：Hello World
来源：http://hz.sysykeji.top/gthfceynkv.html

print("Hello")
来源：http://hz.fengsongda.top/gtmjgaywqj.html

[T32] Lua：局部变量
来源：http://hz.shangyingyoupin.top/gtwhhvawza.html

local a = 1
来源：http://hz.zhiwuduotai.top/gtmkssepdz.html

[T33] Lua：表（数组）
来源：http://hz.ywan-chungtsiang.top/gtbnfuqqhi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.0kj1m.cn/gtqbdlfgon.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtxofdmndh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gtzohujcls.html


<!-- 参考信息 -->