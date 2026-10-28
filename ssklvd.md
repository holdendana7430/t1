代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtuobqsqrz.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtzvzkamyk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtkbukgzec.html

[R37] 把输出赋给变量
来源：http://hz.shzxlz.cn/gtvurzzqec.html

files=$(ls -1)
来源：http://hz.jinqigufen.top/gtkwycgypk.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtgjfkamul.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtqzwldwyr.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtahzxlxmw.html

cmd > out.log 2>&1
来源：http://hz.52xcode.cn/gtaixxuich.html

[R40] 追加写日志
来源：http://hz.ppjwa.cn/gtjanlhsgp.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtyhgligik.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtamybmsnm.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtbfwhnfai.html

[R42] 输入重定向
来源：http://hz.pengpengdd.cyou/gtdpcxfppq.html

wc -l < a.txt
来源：http://hz.xingfuxueyuan.xyz/gtmkebtjnu.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gtoafuuvko.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtndouqvdi.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtwafbzhsp.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtutossccx.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gtkoafoibe.html

find . -name "*.tmp" -delete
来源：http://hz.tian-w.cn/gtzheqnwhz.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtmvdwzpuh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuanzx.com/gtshwlcboa.html

[R47] sed 单行替换
来源：http://hz.hammf.cn/gtgxawyqql.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtrsazlnsg.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtxlvbacyc.html

awk '{print $1, $3}' a.txt
来源：http://hz.sufxvd.cn/gtdsfjjeeg.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtefvmfklk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnqzz.top/gteokvnhyu.html

[R50] awk 求和
来源：http://hz.yuxming.cn/gtwmrbgcfm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtqxwkxjry.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtklvbnigp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sysykeji.top/gtmmjqhxtn.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gtwsydgomn.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtssknsgmg.html

[R53] 查看文件头与实时尾
来源：http://hz.c1oappe.top/gtfttgsrsv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtcvawcwcs.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gtlhbdgspi.html

diff a.txt b.txt
来源：http://hz.shuidangran.top/gtsntjqppe.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtaykfhmfb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtizambeqg.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtvhezfcjn.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtdnksyzir.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gthsfeusoi.html

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtrxrxbdth.html

[R58] 下载文件
来源：http://hz.shanyushiyangkeji.top/gttmefscig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtsrluypvi.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtbahzhcrp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtscptkhrw.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gtqywgmdve.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtycjlgwue.html

[R61] 磁盘占用
来源：http://hz.yj20258888.top/gtpahrmdvf.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtqwprgwvm.html

[R62] 找最占空间的文件
来源：http://hz.316326.xyz/gtnllugxrn.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtnhajduby.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtukbycwxz.html

free -h;  ps aux | grep nginx
来源：http://hz.ywan-chungtsiang.top/gtibasuhqj.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtkfsrddtf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.birdmap.top/gtgtcbqdns.html

[R65] 查看端口占用
来源：http://hz.kuanghao11.cn/gtozznjvqf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtkxpitdcz.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtdpmloeky.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gtuduwfsim.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtxrdaceiv.html

openssl rand -hex 16
来源：http://hz.zhijiandao.cn/gteiigotji.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtlwhngtwo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hywenlv.cn/gtnwxcybqz.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtsepyoxtk.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangdashe.top/gtasmhlmsr.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gtelfnqdsd.html

date +%s;  date -d @1700000000
来源：http://hz.cashguo.top/gtbobrqojw.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtknxifbnx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtsocnekja.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtupjgshej.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gthcrqcpfm.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtebvknpzf.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtwhqmasnj.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtjmejwfdh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtmgkzrxco.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtjlcfegld.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gtfgxjzebt.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtegcbwxvl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtnjdyrcjo.html

[R77] 读取用户输入
来源：http://hz.vqdsnc.cn/gtpebuomrr.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtsmtszadi.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtyvcolvnj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangdashe.top/gtejskpbov.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtjszkjmaf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtzsssiwac.html

[R80] 查看脚本执行耗时
来源：http://hz.zhoulong.xyz/gtkscltbkn.html

time ./run.sh
来源：http://hz.fzhhl.top/gtvcbcinoy.html

================================================================================
来源：http://hz.ybcxt.top/gtminvoksn.html

S. C / C++ 专题
来源：http://hz.0kj1m.cn/gtsvhloqrf.html

================================================================================
来源：http://hz.guowangkeji.top/gtlijchrnd.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtvczfamyh.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtnkrjdwxa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtmnlcuegr.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtnlbrtyst.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtcybbxstw.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtnhbqdbvt.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gttquzzcrh.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtjhpukdgh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtjjbjdbxg.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtbfhferhi.html

strlen(s)
来源：http://hz.yj20258888.top/gttibeoqph.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtyfqcfnbs.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtcrzukvat.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtpcwwwkrn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gtecvfhsyl.html

[S08] C：动态内存分配与释放
来源：http://hz.svipenyu.cn/gtbuvbgnkd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtyexrcsxw.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtlpujprbp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtlulsboso.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtrqmnirgl.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtlviosxry.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtssoxkzpa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.feifeiyinyue.top/gtxgxkrarp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangtech.top/gtoxqeognu.html

fclose(f);
来源：http://hz.c1oappe.top/gtnzbxnvqu.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtwikpbbuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xylfe.cn/gtudykqmmx.html

[S13] C：宏定义
来源：http://hz.daria6918.cn/gtfrlfkzea.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xylfe.cn/gtowlleliu.html

[S14] C：枚举
来源：http://hz.zhaomingkeji.xyz/gtcqqmzsdr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gteowrlgtu.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gthwjpwjtr.html

(double) a / b
来源：http://hz.fengsongda.top/gtvggybmgi.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtbtoeaibp.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtdeavdocc.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtswviqefs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gtlndptvgb.html

[S18] C：命令行参数
来源：http://hz.birdmap.top/gtmxywizgn.html

int main(int argc, char **argv)
来源：http://hz.xinyue.icu/gtjmcvtqeq.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtqauffvjn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtfsmngtbn.html

[S20] C：二分查找
来源：http://hz.cdnleiting.top/gtpafflwyv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtmbnohnxu.html

[S21] C：字符类别判断
来源：http://hz.yangfankeji.com/gtbsptkkol.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtpiqjrolx.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtdmzjdsde.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtjkgvumnt.html

[S23] C：随机数
来源：http://hz.xylfe.cn/gtyexivzmt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtxginhotf.html

[S24] C：获取本地时间
来源：http://hz.zhijiandao.cn/gtuqebntkj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtalkgzvlz.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtgjkyvfkb.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtaunwhzuh.html

[S26] C：内存清零
来源：http://hz.zhoulong.xyz/gtaymaijiv.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtvrkesbty.html

[S27] C：定义常量
来源：http://hz.shangyingyoupin.top/gthyelkmxz.html

const double PI = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtmidgxpwf.html

[S28] C：静态变量
来源：http://hz.yj20258888.top/gthypybtfd.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtcvgkcdro.html

[S29] C：变参函数
来源：http://hz.hysaishi.cn/gtfditcckd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtqpayffbw.html

[S30] C：头文件保护
来源：http://hz.jianghu66.top/gtsoplbagz.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtzresodcu.html

#define X_H
来源：http://hz.dashuyun.cn/gtxaroewew.html

#endif
来源：http://hz.yongpay.top/gtnoajfjpq.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtfpymwsfl.html

#include <iostream>
来源：http://hz.zycfv.cn/gtqnuncprv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shzxlz.cn/gtxgmhyohf.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtaicvlhrn.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtcpleunfd.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtfztfzgmd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.vqdsnc.cn/gtyomszvej.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtzqxbejxy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtqnrjiuss.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtzjondimq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtcaguwbij.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtpdtojvif.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtlrvszhar.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtateulbpt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yongpay.top/gtkrlxgrtb.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gthtyymdxu.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtwavfrbln.html

[S39] C++：自定义比较器排序
来源：http://hz.9152youxi.cn/gtmrmviavi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cheryme.top/gtuqggncco.html

[S40] C++：查找元素
来源：http://hz.vqdsnc.cn/gtabgscnjq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ehwqpu.com/gtmriwmpmq.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtegthflof.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtvvnunrok.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtwuvzxguq.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtugejxybr.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtuegancce.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtiroepjht.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtjrictlav.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtytzqzqlc.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtrgjbpbke.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hnqzz.top/gttpcprndf.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtchlzuwwz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtzifgjgvn.html

[S47] C++：结构化绑定遍历
来源：http://hz.daxiang520.top/gtjaxggjbw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yvedp.cn/gttdqbzadk.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtrkzfhknt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.c1oappe.top/gtkagttdeo.html

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtmefrxudf.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtcyazihov.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtojojuadz.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gtngrshhsw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgufenzy.top/gtwogdwopf.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtkvoaweej.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtjauytpds.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtyrzzdvev.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtwanoduot.html

[S53] C++：移动语义
来源：http://hz.yuanzhike.top/gtolagzwkw.html

std::vector<int> w = std::move(v);
来源：http://hz.jlsjyb.cn/gtpbljdblo.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtkfikkuqt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtxsunyuvt.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtttqvsdrv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtwrcyrdzh.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtkhglzsmo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtiflarnmt.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtdcdyqnzh.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtlqnuodwx.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtdivxdmak.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangshuangyany.cn/gtifrescqt.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtdzmroeup.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtgnokpuqd.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtylqmzdjv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.birdmap.top/gtfuamydcb.html

================================================================================
来源：http://hz.chenzaomai.com/gtbfhhnwfe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtipjfemeq.html

================================================================================
来源：http://hz.ybcxt.top/gtgbbhmhvw.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtgyoiaacy.html

println("Hello")
来源：http://hz.ybcxt.top/gttctksuvv.html

[T02] Kotlin：变量
来源：http://hz.sysykeji.top/gtjetcnsby.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yanxiufei.cn/gtzofhylgo.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtactnrnei.html

"值: $b"
来源：http://hz.yuxming.cn/gtghkoykqi.html

[T04] Kotlin：空安全
来源：http://hz.yangfankeji.com/gtxxdgzxcg.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtqvbdmytk.html

[T05] Kotlin：when 表达式
来源：http://hz.gogol.net.cn/gtwjvwuniu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xinyue.icu/gtenfnniyb.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtdukqpwzk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.snrcjt.cn/gtkmbspkbl.html

[T07] Kotlin：集合过滤
来源：http://hz.cqqwz.cn/gthfwiokvi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtgrrphxnt.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtnawnrjmy.html

data class User(val name: String, val age: Int)
来源：http://hz.nwbrower.top/gtniodmirw.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtqexfptwp.html

fun String.exclaim() = this + "!"
来源：http://hz.gzhubu.top/gthfxutnzi.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtzgxitdva.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yonumen.top/gtzttjgzki.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtrneevuif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jianghu66.top/gthyvwqajv.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtpcofbuwh.html

val (a, b) = Pair(1, 2)
来源：http://hz.svipenyu.cn/gtylaqondx.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtoyddgthm.html

val m = mapOf("a" to 1)
来源：http://hz.tianlin.xyz/gtxkkxkbvb.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtggqszqno.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gtymnyxuzt.html

[T15] Kotlin：接口
来源：http://hz.hongshengwenyu.top/gtuagznfkv.html

interface Shape { fun area(): Double }
来源：http://hz.tianlin.xyz/gtxlximfve.html

[T16] Swift：Hello World
来源：http://hz.316326.xyz/gtwzqbbgwe.html

print("Hello")
来源：http://hz.daxiang520.top/gtaxlelrgd.html

[T17] Swift：变量与常量
来源：http://hz.vqdsnc.cn/gtjcsbveqp.html

var a = 1;  let b = 2
来源：http://hz.xinyue.icu/gtislawzlp.html

[T18] Swift：字符串插值
来源：http://hz.daxiang520.top/gtxjxmgvbu.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtgajohdhv.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtepgoxssq.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtqqguphhr.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtlssdpmrs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtygvvrdqt.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtsrkftacw.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtewwnbzgk.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtyazdumlx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gthydtikvd.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtkcvvykbe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.316326.xyz/gthkbtezmm.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtncqxukuh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gttczqxudw.html

[T25] Swift：结构体
来源：http://hz.aibaodan.cn/gtovtkxzus.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtcxgarsdw.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gthbghbtus.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtslsaunmg.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangkeji.top/gtjojodsva.html

do { try f() } catch { print(error) }
来源：http://hz.jinghuilouyu.cn/gtlbpuanln.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtscwbzhfm.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtezbmxagu.html

[T29] Swift：guard 提前返回
来源：http://hz.birdmap.top/gtcemugkei.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtyhopjjkv.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gtsffwjrbj.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtczmxqvpr.html

[T31] Lua：Hello World
来源：http://hz.jiagoushi.top/gtbebjpyck.html

print("Hello")
来源：http://hz.shzxlz.cn/gtqmltptgt.html

[T32] Lua：局部变量
来源：http://hz.ivvv.top/gtqlggmrju.html

local a = 1
来源：http://hz.gotoacloud.top/gtvndkkkgg.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtpvmtjpuk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shzxlz.cn/gtzdkhsfdu.html

[T34] Lua：遍历表
来源：http://hz.zhiwuduotai.top/gtovvucnqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtbvofhfvt.html

[T35] Lua：字典表
来源：http://hz.ivvv.top/gtxjicebyb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtowzickbu.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtvrcnpjgw.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gtgsxxmjyy.html

[T37] Lua：字符串拼接
来源：http://hz.xinyue.icu/gthtxigggf.html

"a" .. "b"
来源：http://hz.hywenlv.cn/gtxdpvpzac.html

[T38] Lua：条件
来源：http://hz.xuanzx.com/gtygduxyib.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtszjeqeba.html


<!-- 参考信息 -->